# Comparing `tmp/fs_attestation_safe_cli-1.0.7.tar.gz` & `tmp/fs_attestation_safe_cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_attestation_safe_cli-1.0.7.tar", last modified: Mon May  6 08:38:39 2024, max compression
+gzip compressed data, was "fs_attestation_safe_cli-1.0.8.tar", last modified: Mon May  6 15:25:17 2024, max compression
```

## Comparing `fs_attestation_safe_cli-1.0.7.tar` & `fs_attestation_safe_cli-1.0.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.553099 fs_attestation_safe_cli-1.0.7/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 08:38:39.553667 fs_attestation_safe_cli-1.0.7/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.7/README.md
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.506248 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.515403 fs_attestation_safe_cli-1.0.7/safe_cli/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/argparse_validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.516812 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     6461 2024-05-04 05:09:20.000000 fs_attestation_safe_cli-1.0.7/safe_cli/main.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.524676 fs_attestation_safe_cli-1.0.7/safe_cli/operators/
--rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     3344 2024-05-06 08:31:50.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_auth.py
--rw-r--r--   0 mohan      (501) staff       (20)    17956 2024-05-06 08:34:53.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_service_operator.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.532834 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)    46560 2024-05-04 05:19:18.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    25088 2024-05-06 06:17:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/prompt_parser.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)    11341 2024-05-06 06:18:41.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer_constants.py
--rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)     1657 2024-05-06 06:19:12.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-06 08:38:26.000000 fs_attestation_safe_cli-1.0.7/safe_cli/version.py
--rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-06 08:38:39.554832 fs_attestation_safe_cli-1.0.7/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-05-04 05:16:29.000000 fs_attestation_safe_cli-1.0.7/setup.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.548483 fs_attestation_safe_cli-1.0.7/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.552280 fs_attestation_safe_cli-1.0.7/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/balances_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/txs_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_argparse_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_entrypoint.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_cli.py
--rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.361219 fs_attestation_safe_cli-1.0.8/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 15:25:17.361444 fs_attestation_safe_cli-1.0.8/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.8/README.md
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.329697 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-06 15:25:17.000000 fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.336261 fs_attestation_safe_cli-1.0.8/safe_cli/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/argparse_validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.337407 fs_attestation_safe_cli-1.0.8/safe_cli/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/contracts/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6595 2024-05-06 12:47:51.000000 fs_attestation_safe_cli-1.0.8/safe_cli/main.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.341323 fs_attestation_safe_cli-1.0.8/safe_cli/operators/
+-rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3344 2024-05-06 08:31:50.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/fs_attestation_auth.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17956 2024-05-06 08:34:53.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/fs_attestation_service_operator.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.346520 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)    46560 2024-05-06 15:20:49.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18788 2024-05-06 12:44:22.000000 fs_attestation_safe_cli-1.0.8/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    25088 2024-05-06 06:17:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/prompt_parser.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11341 2024-05-06 06:18:41.000000 fs_attestation_safe_cli-1.0.8/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1657 2024-05-06 06:19:12.000000 fs_attestation_safe_cli-1.0.8/safe_cli/safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/safe_cli/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-06 15:24:26.000000 fs_attestation_safe_cli-1.0.8/safe_cli/version.py
+-rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-06 15:25:17.362224 fs_attestation_safe_cli-1.0.8/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-05-04 05:16:29.000000 fs_attestation_safe_cli-1.0.8/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.357100 fs_attestation_safe_cli-1.0.8/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 15:25:17.360722 fs_attestation_safe_cli-1.0.8/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/mocks/balances_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/mocks/txs_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_argparse_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_entrypoint.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_cli.py
+-rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.8/tests/utils.py
```

### Comparing `fs_attestation_safe_cli-1.0.7/LICENSE` & `fs_attestation_safe_cli-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/PKG-INFO` & `fs_attestation_safe_cli-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs_attestation_safe_cli
-Version: 1.0.7
+Version: 1.0.8
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.7/README.md` & `fs_attestation_safe_cli-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/PKG-INFO` & `fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-cli
-Version: 1.0.7
+Version: 1.0.8
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/SOURCES.txt` & `fs_attestation_safe_cli-1.0.8/fs_attestation_safe_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/argparse_validators.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/contracts/safe_to_l2_migration.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/main.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         """
         :param safe_address: Safe address
         :param node_url: Ethereum RPC url
         :param history: If `True` keep command history, otherwise history is not kept after closing the CLI
         """
         self.safe_address = safe_address
         self.node_url = node_url
+        self.safe_tx_service_base_url = safe_tx_service_base_url
         self.fs_attestation_service_base_url = fs_attestation_service_base_url
         if history:
             self.session = PromptSession(
                 history=FileHistory(os.path.join(sys.path[0], ".history"))
             )
         else:
             self.session = PromptSession()
@@ -78,15 +79,15 @@
         """
         split_command = command.split()
         try:
             if (split_command[0]) == "tx-service":
                 print_formatted_text(
                     HTML("<b><ansigreen>Sending txs to tx service</ansigreen></b>")
                 )
-                return SafeTxServiceOperator(self.safe_address, self.node_url)
+                return SafeTxServiceOperator(self.safe_address, self.node_url, self.safe_tx_service_base_url)
             elif split_command[0] == "blockchain":
                 print_formatted_text(
                     HTML("<b><ansigreen>Sending txs to blockchain</ansigreen></b>")
                 )
                 return self.safe_operator
         except SafeServiceNotAvailable:
             print_formatted_text(
@@ -107,15 +108,15 @@
             try:
                 command = self.get_command()
                 if not command.strip():
                     continue
 
                 new_operator = self.parse_operator_mode(command)
                 if new_operator:
-                    self.prompt_parser = PromptParser(new_operator)
+                    self.prompt_parser = PromptParser(new_operator, self.fs_attestation_service_operator)
                     new_operator.refresh_safe_cli_info()  # ClI info needs to be initialized
                 else:
                     self.prompt_parser.process_command(command)
             except EOFError:
                 break
             except KeyboardInterrupt:
                 continue
```

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/exceptions.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_auth.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/fs_attestation_auth.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_service_operator.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/fs_attestation_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_wallet.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_wallet.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_operator.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/operators/safe_tx_service_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from . import SafeServiceNotAvailable
 from .exceptions import AccountNotLoadedException, NonExistingOwnerException
 from .hw_wallets.hw_wallet import HwWallet
 from .safe_operator import SafeOperator
 
 
 class SafeTxServiceOperator(SafeOperator):
-    def __init__(self, address: str, node_url: str):
-        super().__init__(address, node_url)
+    def __init__(self, address: str, node_url: str, safe_tx_service_base_url: str):
+        super().__init__(address, node_url, safe_tx_service_base_url)
         if not self.safe_tx_service:
             raise SafeServiceNotAvailable(
                 f"Cannot configure tx service for network {self.network.name}"
             )
         self.require_all_signatures = (
             False  # It doesn't require all signatures to be present to send a tx
         )
```

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/prompt_parser.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/safe_addresses.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer_constants.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/safe_completer_constants.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/safe_creator.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/safe_lexer.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/safe_cli/utils.py` & `fs_attestation_safe_cli-1.0.8/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/setup.cfg` & `fs_attestation_safe_cli-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/setup.py` & `fs_attestation_safe_cli-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/mocks/balances_mock.py` & `fs_attestation_safe_cli-1.0.8/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/mocks/data_decoded_mock.py` & `fs_attestation_safe_cli-1.0.8/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/mocks/multisig_tx_mock.py` & `fs_attestation_safe_cli-1.0.8/tests/mocks/multisig_tx_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/mocks/txs_mock.py` & `fs_attestation_safe_cli-1.0.8/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/safe_cli_test_case_mixin.py` & `fs_attestation_safe_cli-1.0.8/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_argparse_validators.py` & `fs_attestation_safe_cli-1.0.8/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_entrypoint.py` & `fs_attestation_safe_cli-1.0.8/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.8/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.8/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_ledger_wallet.py` & `fs_attestation_safe_cli-1.0.8/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_addresses.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_cli.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_completer.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_creator.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_lexer.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_operator.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.8/tests/test_safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_trezor_wallet.py` & `fs_attestation_safe_cli-1.0.8/tests/test_trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/test_utils.py` & `fs_attestation_safe_cli-1.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.7/tests/utils.py` & `fs_attestation_safe_cli-1.0.8/tests/utils.py`

 * *Files identical despite different names*

