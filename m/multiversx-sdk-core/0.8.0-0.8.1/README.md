# Comparing `tmp/multiversx_sdk_core-0.8.0.tar.gz` & `tmp/multiversx_sdk_core-0.8.1.tar.gz`

## Comparing `multiversx_sdk_core-0.8.0.tar` & `multiversx_sdk_core-0.8.1.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/py.typed
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/pyrightconfig.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/requirements-dev.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.github/release.yml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.vscode/settings.json
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/account.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/account_test.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/address.py
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/address_test.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/bech32.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/code_metadata.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/code_metadata_test.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/codec.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/constants.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query_builder.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query_builder_test.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/errors.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/interfaces.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/message.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/message_test.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/serializer.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/token_payment.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/token_payment_test.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/tokens.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/tokens_test.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_payload.py
--rw-r--r--   0        0        0     9727 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_test.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/typecheck.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction.proto
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_pb2.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_pb2.pyi
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_serializer.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_serializer_test.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/wallets.py
--rwxr-xr-x   0        0        0      687 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testdata/adder.wasm
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testwallets/alice.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testwallets/bob.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testwallets/carol.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testwallets/frank.pem
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testwallets/grace.pem
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/__init__.py
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/contract_builders.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/contract_builders_test.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/default_configuration.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/default_configuration_test.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/esdt_builders.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/other_builders.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transaction_builder.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transfers_builders.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/__init__.py
--rw-r--r--   0        0        0    15688 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/delegation_transactions_factory.py
--rw-r--r--   0        0        0    17971 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/delegation_transactions_factory_test.py
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/relayed_transactions_factory.py
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/relayed_transactions_factory_test.py
--rw-r--r--   0        0        0     9553 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/smart_contract_transaction_factory_test.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/smart_contract_transactions_factory.py
--rw-r--r--   0        0        0    21397 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_management_transactions_factory.py
--rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_management_transactions_factory_test.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_transfers_data_builder.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transaction_builder.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transactions_factory_config.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transfer_transactions_factory.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transfer_transactions_factory_test.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/interfaces.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/LICENSE
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/README.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/py.typed
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/pyrightconfig.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/requirements-dev.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.github/release.yml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/account.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/account_test.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/address.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/address_test.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/bech32.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/code_metadata.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/code_metadata_test.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/codec.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/codec_test.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/constants.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query_builder.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query_builder_test.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/errors.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/interfaces.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/message.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/message_test.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/serializer.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/token_payment.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/token_payment_test.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/tokens.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/tokens_test.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_payload.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_test.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/typecheck.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction.proto
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_pb2.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_pb2.pyi
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_serializer.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_serializer_test.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/wallets.py
+-rwxr-xr-x   0        0        0      687 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testdata/adder.wasm
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testwallets/alice.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testwallets/bob.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testwallets/carol.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testwallets/frank.pem
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testwallets/grace.pem
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/__init__.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/contract_builders.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/contract_builders_test.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/default_configuration.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/default_configuration_test.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/esdt_builders.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/other_builders.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transaction_builder.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transfers_builders.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/__init__.py
+-rw-r--r--   0        0        0    15688 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/delegation_transactions_factory.py
+-rw-r--r--   0        0        0    17971 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/delegation_transactions_factory_test.py
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/relayed_transactions_factory.py
+-rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/relayed_transactions_factory_test.py
+-rw-r--r--   0        0        0     9553 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/smart_contract_transaction_factory_test.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/smart_contract_transactions_factory.py
+-rw-r--r--   0        0        0    21397 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_management_transactions_factory.py
+-rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_management_transactions_factory_test.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_transfers_data_builder.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transaction_builder.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transactions_factory_config.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transfer_transactions_factory.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transfer_transactions_factory_test.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/interfaces.py
+-rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/README.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.8.1/PKG-INFO
```

### Comparing `multiversx_sdk_core-0.8.0/.github/workflows/linter-flake8.yml` & `multiversx_sdk_core-0.8.1/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/.github/workflows/linter-pyright.yml` & `multiversx_sdk_core-0.8.1/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/.github/workflows/python-publish.yml` & `multiversx_sdk_core-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/.github/workflows/test.yml` & `multiversx_sdk_core-0.8.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/__init__.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/address.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/address.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/address_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/address_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/bech32.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/bech32.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/code_metadata.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/code_metadata.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/code_metadata_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/code_metadata_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/constants.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/constants.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/contract_query_builder_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/contract_query_builder_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 def test_contract_query_builder():
     contract = Address.new_from_bech32("erd1qqqqqqqqqqqqqpgquzmh78klkqwt0p4rjys0qtp3la07gz4d396qn50nnm")
     caller = Address.new_from_bech32("erd1qyu5wthldzr8wx5c9ucg8kjagg0jfs53s8nr3zpz3hypefsdd8ssycr6th")
 
     builder = ContractQueryBuilder(
         contract=contract,
         function="getFoobar",
-        call_arguments=[42, "test"],
+        call_arguments=[42, "test", -836623209073744937290891644],
         caller=caller,
         value=1
     )
 
     query = builder.build()
 
     assert query.contract == contract
     assert query.function == "getFoobar"
-    assert query.encoded_arguments == ["2a", "74657374"]
+    assert query.encoded_arguments == ["2a", "74657374", "fd4bf624f561bc2894c6fe84"]
     assert query.caller == caller
     assert query.value == 1
```

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/errors.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/interfaces.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/message.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/message.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/serializer.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/serializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List, Protocol, Sequence, runtime_checkable
 
-from multiversx_sdk_core.codec import encode_unsigned_number
+from multiversx_sdk_core.codec import encode_unsigned_number, encode_signed_number
 from multiversx_sdk_core.constants import ARGS_SEPARATOR
 from multiversx_sdk_core.errors import ErrCannotSerializeArgument
 
 
 @runtime_checkable
 class IArgument(Protocol):
     def serialize(self) -> bytes: ...
@@ -29,14 +29,16 @@
     return buffer.hex()
 
 
 def arg_to_buffer(arg: Any) -> bytes:
     if isinstance(arg, str):
         return arg.encode("utf-8")
     if isinstance(arg, int):
+        if arg < 0:
+            return encode_signed_number(arg)
         return encode_unsigned_number(arg)
     if isinstance(arg, bytes):
         return arg
     if isinstance(arg, bytearray):
         return bytes(arg)
     if isinstance(arg, IArgument):
         return arg.serialize()
```

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/token_payment.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/token_payment.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/token_payment_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/token_payment_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/tokens.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/tokens.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/tokens_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/tokens_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from base64 import b64encode
 from collections import OrderedDict
 from hashlib import blake2b
 from typing import Any, Dict, Optional, Protocol
 
+from Cryptodome.Hash import keccak
+
 from multiversx_sdk_core.constants import (DEFAULT_HRP, DIGEST_SIZE,
                                            TRANSACTION_MIN_GAS_PRICE,
                                            TRANSACTION_OPTIONS_DEFAULT,
                                            TRANSACTION_VERSION_DEFAULT)
 from multiversx_sdk_core.errors import NotEnoughGasError
 from multiversx_sdk_core.interfaces import INetworkConfig, ITransaction
 from multiversx_sdk_core.proto.transaction_serializer import ProtoSerializer
@@ -83,14 +85,17 @@
         return int(fee_for_move + processing_fee)
 
     def compute_bytes_for_signing(self, transaction: ITransaction) -> bytes:
         dictionary = self._to_dictionary(transaction)
         serialized = self._dict_to_json(dictionary)
         return serialized
 
+    def compute_hash_for_signing(self, transaction: ITransaction) -> bytes:
+        return keccak.new(digest_bits=256).update(self.compute_bytes_for_signing(transaction)).digest()
+
     def compute_transaction_hash(self, transaction: ITransaction) -> bytes:
         proto = ProtoSerializer()
         serialized_tx = proto.serialize_transaction(transaction)
         tx_hash = blake2b(serialized_tx, digest_size=DIGEST_SIZE).hexdigest()
         return bytes.fromhex(tx_hash)
 
     def _to_dictionary(self, transaction: ITransaction) -> Dict[str, Any]:
```

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_payload.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_payload.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,7 +187,23 @@
 
         proto_serializer = ProtoSerializer()
         serialized = proto_serializer.serialize_transaction(transaction)
         assert serialized.hex() == "085c120e00018ee90ff6181f3761632000001a208049d639e5a6980d1cd2392abcce41029cda74a1563523a202f09641cc2618f82a200139472eff6886771a982f3083da5d421f24c29181e63888228dc81ca60d69e1388094ebdc0340f093094a0f746573742064617461206669656c64520d6c6f63616c2d746573746e657458026240e574d78b19e1481a6b9575c162e66f2f906a3178aec537509356385c4f1a5330a9b73a87a456fc6d7041e93b5f8a1231a92fb390174872a104a0929215600c0c6802722032a3f14cf53c4d0543954f6cf1bda0369d13e661dec095107627dc0f6d33612f7a4000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"
 
         tx_hash = self.transaction_computer.compute_transaction_hash(transaction)
         assert tx_hash.hex() == "242022e9dcfa0ee1d8199b0043314dbda8601619f70069ebc441b9f03349a35c"
+
+    def test_sign_transaction_by_hash(self):
+        tx = Transaction(
+            sender="erd1qyu5wthldzr8wx5c9ucg8kjagg0jfs53s8nr3zpz3hypefsdd8ssycr6th",
+            receiver="erd1spyavw0956vq68xj8y4tenjpq2wd5a9p2c6j8gsz7ztyrnpxrruqzu66jx",
+            value=0,
+            gas_limit=50000,
+            version=2,
+            options=1,
+            chain_id="integration tests chain ID",
+            nonce=89
+        )
+        serialized = self.transaction_computer.compute_hash_for_signing(tx)
+        tx.signature = self.alice.secret_key.sign(serialized)
+
+        assert tx.signature.hex() == "f0c81f2393b1ec5972c813f817bae8daa00ade91c6f75ea604ab6a4d2797aca4378d783023ff98f1a02717fe4f24240cdfba0b674ee9abb18042203d713bc70a"
```

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/typecheck.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/typecheck.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction.proto` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction.proto`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_pb2.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_pb2.pyi` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_serializer.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_serializer.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/proto/transaction_serializer_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/proto/transaction_serializer_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/wallets.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/testutils/testdata/adder.wasm` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/testutils/testdata/adder.wasm`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/__init__.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/contract_builders.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/contract_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/contract_builders_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/contract_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/default_configuration.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/default_configuration.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/esdt_builders.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/esdt_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/esdt_builders_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/esdt_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v1_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v1_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v2_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/relayed_v2_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transaction_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transfers_builders.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transfers_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_builders/transfers_builders_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_builders/transfers_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/__init__.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/delegation_transactions_factory.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/delegation_transactions_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/delegation_transactions_factory_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/delegation_transactions_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/relayed_transactions_factory.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/relayed_transactions_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/relayed_transactions_factory_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/relayed_transactions_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/smart_contract_transaction_factory_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/smart_contract_transaction_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/smart_contract_transactions_factory.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/smart_contract_transactions_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_management_transactions_factory.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_management_transactions_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_management_transactions_factory_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_management_transactions_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/token_transfers_data_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/token_transfers_data_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transaction_builder.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transactions_factory_config.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transactions_factory_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transfer_transactions_factory.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transfer_transactions_factory.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_factories/transfer_transactions_factory_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_factories/transfer_transactions_factory_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/interfaces.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/token_operations_outcome_parser_types.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py` & `multiversx_sdk_core-0.8.1/multiversx_sdk_core/transaction_parsers/transaction_on_network_wrapper.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/.gitignore` & `multiversx_sdk_core-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/LICENSE` & `multiversx_sdk_core-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/README.md` & `multiversx_sdk_core-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.8.0/pyproject.toml` & `multiversx_sdk_core-0.8.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-core"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Core components of the MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "pycryptodomex==3.16.0",
-  "protobuf==3.20.1"
+  "pycryptodomex==3.19.1",
+  "protobuf==3.20.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/multiversx/mx-sdk-py-core"
```

### Comparing `multiversx_sdk_core-0.8.0/PKG-INFO` & `multiversx_sdk_core-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: multiversx-sdk-core
-Version: 0.8.0
+Version: 0.8.1
 Summary: Core components of the MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-core
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: protobuf==3.20.1
-Requires-Dist: pycryptodomex==3.16.0
+Requires-Dist: protobuf==3.20.2
+Requires-Dist: pycryptodomex==3.19.1
 Description-Content-Type: text/markdown
 
 # mx-sdk-py-core
 
 Core components of the MultiversX Python SDK.
 
 ## Distribution
```

