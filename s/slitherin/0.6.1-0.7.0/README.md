# Comparing `tmp/slitherin-0.6.1.tar.gz` & `tmp/slitherin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slitherin-0.6.1.tar", last modified: Wed Mar 13 11:51:08 2024, max compression
+gzip compressed data, was "slitherin-0.7.0.tar", last modified: Tue May  7 10:11:05 2024, max compression
```

## Comparing `slitherin-0.6.1.tar` & `slitherin-0.7.0.tar`

### file list

```diff
@@ -1,96 +1,113 @@
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.919462 slitherin-0.6.1/
--rw-r--r--   0 ndkirillov   (501) staff       (20)    34523 2023-10-30 05:01:14.000000 slitherin-0.6.1/LICENSE.txt
--rw-r--r--   0 ndkirillov   (501) staff       (20)       30 2023-12-06 13:12:42.000000 slitherin-0.6.1/MANIFEST.in
--rw-r--r--   0 ndkirillov   (501) staff       (20)    23817 2024-03-13 11:51:08.919276 slitherin-0.6.1/PKG-INFO
--rw-r--r--   0 ndkirillov   (501) staff       (20)    23251 2024-03-13 09:41:11.000000 slitherin-0.6.1/README.md
--rw-r--r--   0 ndkirillov   (501) staff       (20)       38 2024-03-13 11:51:08.919498 slitherin-0.6.1/setup.cfg
--rw-r--r--   0 ndkirillov   (501) staff       (20)     1164 2024-02-15 10:13:32.000000 slitherin-0.6.1/setup.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.907911 slitherin-0.6.1/slitherin/
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2693 2024-03-13 11:48:31.000000 slitherin-0.6.1/slitherin/__init__.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.909109 slitherin-0.6.1/slitherin/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3196 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     8263 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)      241 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin/__pycache__/consts.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     5232 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/cli.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)       64 2024-03-13 11:48:31.000000 slitherin-0.6.1/slitherin/consts.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.913514 slitherin-0.6.1/slitherin/detectors/
--rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/__init__.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.916322 slitherin-0.6.1/slitherin/detectors/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)      181 2023-12-06 13:12:59.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2031 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/before_token_transfer.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     6761 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/call_forward_to_protected.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3159 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/double_entry_token_possibility.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     5132 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/dubious_typecast.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4884 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/ecrecover.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2977 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/event_setter.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3591 2023-12-07 16:24:06.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/falsy_only_eoa_modifier.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     5926 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/for_continue_increment.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4379 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/inconsistent_nonreentrant.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4433 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/magic_number.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3510 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/multiple_storage_read.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4897 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/nft_approve_warning.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     9649 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/potential_arith_overflow.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2998 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/public_vs_external.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)    21921 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/read_only_reentrancy.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     5109 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/strange_setter.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3858 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/timelock_controller.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2395 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/token_fallback.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2645 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/tx_gasprice_warning.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)    26306 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/uni_v2.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4472 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/unprotected_initialize.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3496 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/__pycache__/unprotected_setter.cpython-311.pyc
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.916500 slitherin-0.6.1/slitherin/detectors/aave/
--rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/aave/__init__.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.916747 slitherin-0.6.1/slitherin/detectors/aave/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)      186 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/aave/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4638 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/aave/__pycache__/flashloan_callback.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3990 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/aave/flashloan_callback.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.916915 slitherin-0.6.1/slitherin/detectors/arbitrary_call/
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.917215 slitherin-0.6.1/slitherin/detectors/arbitrary_call/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)     9314 2023-12-07 16:24:05.000000 slitherin-0.6.1/slitherin/detectors/arbitrary_call/__pycache__/arbitrary_call.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     9136 2023-12-07 16:22:50.000000 slitherin-0.6.1/slitherin/detectors/arbitrary_call/arbitrary_call.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.917630 slitherin-0.6.1/slitherin/detectors/arbitrum/
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.918182 slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4502 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/arbitrum_prevrandao_difficulty.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4657 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/block_number_timestamp.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2981 2024-02-15 10:15:18.000000 slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/solidity_version.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3128 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3328 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/arbitrum/block_number_timestamp.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     1888 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/before_token_transfer.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3980 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/call_forward_to_protected.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2045 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/double_entry_token_possibility.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3915 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/dubious_typecast.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4239 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/ecrecover.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     1877 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/event_setter.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2401 2023-12-07 16:22:50.000000 slitherin-0.6.1/slitherin/detectors/falsy_only_eoa_modifier.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4677 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/for_continue_increment.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3051 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/inconsistent_nonreentrant.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3182 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/magic_number.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2522 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/multiple_storage_read.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3110 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/nft_approve_warning.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     7621 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/potential_arith_overflow.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2117 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/public_vs_external.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)    17933 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/read_only_reentrancy.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.918486 slitherin-0.6.1/slitherin/detectors/reentrancy/
--rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/reentrancy/__init__.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.918785 slitherin-0.6.1/slitherin/detectors/reentrancy/__pycache__/
--rw-r--r--   0 ndkirillov   (501) staff       (20)      192 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/reentrancy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)    16807 2023-12-06 13:13:00.000000 slitherin-0.6.1/slitherin/detectors/reentrancy/__pycache__/reentrancy.cpython-311.pyc
--rw-r--r--   0 ndkirillov   (501) staff       (20)    10769 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/reentrancy/reentrancy.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     4488 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/strange_setter.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2817 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/timelock_controller.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     1645 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/token_fallback.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     1855 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/tx_gasprice_warning.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)    22658 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/uni_v2.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3212 2024-02-15 10:13:32.000000 slitherin-0.6.1/slitherin/detectors/unprotected_initialize.py
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2842 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/detectors/unprotected_setter.py
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.919039 slitherin-0.6.1/slitherin/utils/
--rw-r--r--   0 ndkirillov   (501) staff       (20)     2599 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/utils/deflat_tokens.json
--rw-r--r--   0 ndkirillov   (501) staff       (20)      735 2023-12-06 13:12:42.000000 slitherin-0.6.1/slitherin/utils/rebase_tokens.json
-drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-03-13 11:51:08.908702 slitherin-0.6.1/slitherin.egg-info/
--rw-r--r--   0 ndkirillov   (501) staff       (20)    23817 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/PKG-INFO
--rw-r--r--   0 ndkirillov   (501) staff       (20)     3953 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/SOURCES.txt
--rw-r--r--   0 ndkirillov   (501) staff       (20)        1 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/dependency_links.txt
--rw-r--r--   0 ndkirillov   (501) staff       (20)      126 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/entry_points.txt
--rw-r--r--   0 ndkirillov   (501) staff       (20)       25 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/requires.txt
--rw-r--r--   0 ndkirillov   (501) staff       (20)       10 2024-03-13 11:51:08.000000 slitherin-0.6.1/slitherin.egg-info/top_level.txt
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.551403 slitherin-0.7.0/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    34523 2023-10-30 05:01:14.000000 slitherin-0.7.0/LICENSE.txt
+-rw-r--r--   0 ndkirillov   (501) staff       (20)       30 2024-03-22 08:34:33.000000 slitherin-0.7.0/MANIFEST.in
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    24396 2024-05-07 10:11:05.551175 slitherin-0.7.0/PKG-INFO
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    23830 2024-05-07 10:08:30.000000 slitherin-0.7.0/README.md
+-rw-r--r--   0 ndkirillov   (501) staff       (20)       38 2024-05-07 10:11:05.551440 slitherin-0.7.0/setup.cfg
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1237 2024-05-07 10:08:30.000000 slitherin-0.7.0/setup.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.540823 slitherin-0.7.0/slitherin/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3292 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/__init__.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.541930 slitherin-0.7.0/slitherin/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3806 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     8263 2024-03-22 09:42:01.000000 slitherin-0.7.0/slitherin/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      241 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/__pycache__/consts.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5232 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/cli.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)       64 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/consts.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.544545 slitherin-0.7.0/slitherin/detectors/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/__init__.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.547436 slitherin-0.7.0/slitherin/detectors/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      181 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2031 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/before_token_transfer.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     6761 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/call_forward_to_protected.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3159 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/double_entry_token_possibility.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5132 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/dubious_typecast.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4884 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/ecrecover.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2977 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/event_setter.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3591 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/falsy_only_eoa_modifier.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5926 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/for_continue_increment.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4379 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/inconsistent_nonreentrant.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4433 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/magic_number.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3510 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/multiple_storage_read.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5583 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/nft_approve_warning.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     9715 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/potential_arith_overflow.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5157 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/price_manipulation.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2998 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/public_vs_external.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    21936 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/read_only_reentrancy.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5860 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/strange_setter.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3858 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/timelock_controller.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2395 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/token_fallback.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2645 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/tx_gasprice_warning.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    26306 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/uni_v2.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4472 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/unprotected_initialize.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3496 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/__pycache__/unprotected_setter.cpython-311.pyc
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.547620 slitherin-0.7.0/slitherin/detectors/aave/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/aave/__init__.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.547829 slitherin-0.7.0/slitherin/detectors/aave/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      186 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/aave/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4638 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/aave/__pycache__/flashloan_callback.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3990 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/aave/flashloan_callback.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.547972 slitherin-0.7.0/slitherin/detectors/arbitrary_call/
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.548136 slitherin-0.7.0/slitherin/detectors/arbitrary_call/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     9314 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/arbitrary_call/__pycache__/arbitrary_call.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     9136 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/arbitrary_call/arbitrary_call.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.548557 slitherin-0.7.0/slitherin/detectors/arbitrum/
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.549115 slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3607 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/arbitrum_chainlink_price_feed.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4507 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/arbitrum_prevrandao_difficulty.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4662 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/block_number_timestamp.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2981 2024-02-15 10:15:18.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/solidity_version.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2579 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/arbitrum_chainlink_price_feed.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3135 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3335 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/arbitrum/block_number_timestamp.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.549538 slitherin-0.7.0/slitherin/detectors/balancer/
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.549685 slitherin-0.7.0/slitherin/detectors/balancer/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5659 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/balancer/__pycache__/balancer_readonly_reentrancy.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4298 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/balancer/balancer_readonly_reentrancy.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1888 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/before_token_transfer.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3980 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/call_forward_to_protected.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.549827 slitherin-0.7.0/slitherin/detectors/curve/
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.549971 slitherin-0.7.0/slitherin/detectors/curve/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5236 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/curve/__pycache__/curve_readonly_reentrancy.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4132 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/curve/curve_readonly_reentrancy.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2045 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/double_entry_token_possibility.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3915 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/dubious_typecast.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4239 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/ecrecover.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1877 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/event_setter.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2401 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/falsy_only_eoa_modifier.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4677 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/for_continue_increment.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3051 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/inconsistent_nonreentrant.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3182 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/magic_number.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2522 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/multiple_storage_read.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3730 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/nft_approve_warning.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     7652 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/potential_arith_overflow.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3783 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/price_manipulation.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2117 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/public_vs_external.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    17952 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/read_only_reentrancy.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.550193 slitherin-0.7.0/slitherin/detectors/reentrancy/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)        0 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/reentrancy/__init__.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.550474 slitherin-0.7.0/slitherin/detectors/reentrancy/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      192 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/reentrancy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    16807 2024-03-22 09:33:53.000000 slitherin-0.7.0/slitherin/detectors/reentrancy/__pycache__/reentrancy.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    10769 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/reentrancy/reentrancy.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     5201 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/strange_setter.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2817 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/timelock_controller.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1645 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/token_fallback.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1855 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/tx_gasprice_warning.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    22658 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/uni_v2.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     3212 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/unprotected_initialize.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2842 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/detectors/unprotected_setter.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.550599 slitherin-0.7.0/slitherin/detectors/vyper/
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.550708 slitherin-0.7.0/slitherin/detectors/vyper/__pycache__/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2962 2024-05-07 10:09:48.000000 slitherin-0.7.0/slitherin/detectors/vyper/__pycache__/reentrancy_curve_vyper_version.cpython-311.pyc
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     1967 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/detectors/vyper/reentrancy_curve_vyper_version.py
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      472 2024-05-07 10:08:30.000000 slitherin-0.7.0/slitherin/napalm.py
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.550919 slitherin-0.7.0/slitherin/utils/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     2599 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/utils/deflat_tokens.json
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      735 2024-03-22 08:34:33.000000 slitherin-0.7.0/slitherin/utils/rebase_tokens.json
+drwxr-xr-x   0 ndkirillov   (501) staff       (20)        0 2024-05-07 10:11:05.541554 slitherin-0.7.0/slitherin.egg-info/
+-rw-r--r--   0 ndkirillov   (501) staff       (20)    24396 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/PKG-INFO
+-rw-r--r--   0 ndkirillov   (501) staff       (20)     4658 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/SOURCES.txt
+-rw-r--r--   0 ndkirillov   (501) staff       (20)        1 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/dependency_links.txt
+-rw-r--r--   0 ndkirillov   (501) staff       (20)      188 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/entry_points.txt
+-rw-r--r--   0 ndkirillov   (501) staff       (20)       25 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/requires.txt
+-rw-r--r--   0 ndkirillov   (501) staff       (20)       10 2024-05-07 10:11:05.000000 slitherin-0.7.0/slitherin.egg-info/top_level.txt
```

### Comparing `slitherin-0.6.1/LICENSE.txt` & `slitherin-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/PKG-INFO` & `slitherin-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: slitherin
-Version: 0.6.1
+Version: 0.7.0
 Summary: Pessimistic security Slither detectors
 Home-page: https://github.com/pessimistic-io/slitherin
 Author: Pessimistic.io
 Author-email: info@pessimistic.io
 License: AGPL-3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: slither-analyzer>=0.10.0
 
-#  Slitherin by Pessimistic.io
+# Slitherin by Pessimistic.io
 
 [![Blog](https://img.shields.io/badge/Blog-Link-blue?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://blog.pessimistic.io/)
 [![Our Website](https://img.shields.io/badge/By-pessimistic.io-green?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://pessimistic.io/)
 [![Mail](https://img.shields.io/badge/Mail-gm%40pessimistic.io-orange?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](mailto:gm@pessimistic.io)
 
 **Welcome!** We are the [pessimistic.io](https://pessimistic.io/) team, and in recent months we have been actively developing our [own **Slither detectors**](https://github.com/pessimistic-io/slitherin/tree/develop/slitherin/detectors) to help with code review and audit process. This repository contains everything you may require to work with them!
 
@@ -112,14 +112,15 @@
 | [Call Forward To Protected](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/call_forward_to_protected.py)                  | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/call_forward_to_protected.md)             | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/call_forward_to_protected_test.sol)                                                  | 0                                                                                                                |
 | [Before Token Transfer](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/before_token_transfer.py)                          | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/before_token_transfer.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/before_token_transfer_test.sol)                                                      | 2                                                                                                                |
 | [For Continue Increment](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/for_continue_increment.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/for_continue_increment.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/for_continue_increment.sol)                                                         | 0                                                                                                                |
 | [AAVE Flasloan Callback](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/aave/flashloan_callback.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/aave/flashloan_callback.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/AaveFlashloanCallback.sol)                                                         | 0                                                                                                                |
 | [Arbitrary Call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/arbitrary_call.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/arbitrary_call_test.sol)                                                         | 0                                                                                                                |
 | [Elliptic Curve Recover](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/ecrecover.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/ecrecover.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/ecrecover.sol)                                                         | 0                                                                                                                |
 | [Public vs External](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/public_vs_external.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/public_vs_external.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/public_vs_external_test.sol)                                                         | 0                                                                                                                |
+| [Balancer Read-only Reentrancy](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/balancer/balancer_readonly_reentrancy.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/balancer/readonly_reentrancy.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/balancer/readonly_reentrancy_test.sol)                                                         | 0                                                                                                                |
 
 **Please note:**
 
 - *Valid - issues included in reports and fixed by developers (January 2023 - June 2023).
 
 - There are two detectors which have several checks inside: [pess-uni-v2](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/uni_v2.py) and [arbitrary-call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py).
```

### Comparing `slitherin-0.6.1/README.md` & `slitherin-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Slitherin by Pessimistic.io
+# Slitherin by Pessimistic.io
 
 [![Blog](https://img.shields.io/badge/Blog-Link-blue?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://blog.pessimistic.io/)
 [![Our Website](https://img.shields.io/badge/By-pessimistic.io-green?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://pessimistic.io/)
 [![Mail](https://img.shields.io/badge/Mail-gm%40pessimistic.io-orange?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](mailto:gm@pessimistic.io)
 
 **Welcome!** We are the [pessimistic.io](https://pessimistic.io/) team, and in recent months we have been actively developing our [own **Slither detectors**](https://github.com/pessimistic-io/slitherin/tree/develop/slitherin/detectors) to help with code review and audit process. This repository contains everything you may require to work with them!
 
@@ -95,14 +95,15 @@
 | [Call Forward To Protected](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/call_forward_to_protected.py)                  | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/call_forward_to_protected.md)             | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/call_forward_to_protected_test.sol)                                                  | 0                                                                                                                |
 | [Before Token Transfer](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/before_token_transfer.py)                          | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/before_token_transfer.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/before_token_transfer_test.sol)                                                      | 2                                                                                                                |
 | [For Continue Increment](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/for_continue_increment.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/for_continue_increment.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/for_continue_increment.sol)                                                         | 0                                                                                                                |
 | [AAVE Flasloan Callback](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/aave/flashloan_callback.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/aave/flashloan_callback.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/AaveFlashloanCallback.sol)                                                         | 0                                                                                                                |
 | [Arbitrary Call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/arbitrary_call.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/arbitrary_call_test.sol)                                                         | 0                                                                                                                |
 | [Elliptic Curve Recover](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/ecrecover.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/ecrecover.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/ecrecover.sol)                                                         | 0                                                                                                                |
 | [Public vs External](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/public_vs_external.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/public_vs_external.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/public_vs_external_test.sol)                                                         | 0                                                                                                                |
+| [Balancer Read-only Reentrancy](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/balancer/balancer_readonly_reentrancy.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/balancer/readonly_reentrancy.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/balancer/readonly_reentrancy_test.sol)                                                         | 0                                                                                                                |
 
 **Please note:**
 
 - *Valid - issues included in reports and fixed by developers (January 2023 - June 2023).
 
 - There are two detectors which have several checks inside: [pess-uni-v2](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/uni_v2.py) and [arbitrary-call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py).
```

### Comparing `slitherin-0.6.1/setup.py` & `slitherin-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,11 @@
     install_requires=["slither-analyzer>=0.10.0"],
     extras_requires={
         "dev": ["twine>=4.0.2"],
     },
     entry_points={
         "slither_analyzer.plugin": "slither slitherin-plugins=slitherin:make_plugin",
         "console_scripts": ["slitherin=slitherin.cli:main"],
+        "napalm.collection": ["slitherin=slitherin.napalm:entry_point"],
     },
     include_package_data=True,
 )
```

### Comparing `slitherin-0.6.1/slitherin/__init__.py` & `slitherin-0.7.0/slitherin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,19 +25,25 @@
 from slitherin.detectors.aave.flashloan_callback import AAVEFlashloanCallbackDetector
 from slitherin.detectors.arbitrum.arbitrum_prevrandao_difficulty import (
     ArbitrumPrevrandaoDifficulty,
 )
 from slitherin.detectors.arbitrum.block_number_timestamp import (
     ArbitrumBlockNumberTimestamp,
 )
+from slitherin.detectors.arbitrum.arbitrum_chainlink_price_feed import ArbitrumChainlinkPriceFeed
 from slitherin.detectors.potential_arith_overflow import PotentialArithmOverflow
+from slitherin.detectors.curve.curve_readonly_reentrancy import CurveReadonlyReentrancy
+from slitherin.detectors.balancer.balancer_readonly_reentrancy import BalancerReadonlyReentrancy
+from slitherin.detectors.vyper.reentrancy_curve_vyper_version import CurveVyperReentrancy
+from slitherin.detectors.price_manipulation import PriceManipulationDetector
 
 artbitrum_detectors = [
     ArbitrumPrevrandaoDifficulty,
     ArbitrumBlockNumberTimestamp,
+    ArbitrumChainlinkPriceFeed
 ]
 
 plugin_detectors = artbitrum_detectors + [
     DoubleEntryTokenPossiblity,
     UnprotectedSetter,
     NftApproveWarning,
     InconsistentNonreentrant,
@@ -56,14 +62,18 @@
     UniswapV2,
     TokenFallback,
     ForContinueIncrement,
     ArbitraryCall,
     Ecrecover,
     PublicVsExternal,
     AAVEFlashloanCallbackDetector,
-    PotentialArithmOverflow
+    PotentialArithmOverflow,
+    CurveReadonlyReentrancy,
+    BalancerReadonlyReentrancy,
+    CurveVyperReentrancy,
+    PriceManipulationDetector
 ]
 plugin_printers = []
 
 
 def make_plugin():
     return plugin_detectors, plugin_printers
```

### Comparing `slitherin-0.6.1/slitherin/__pycache__/__init__.cpython-311.pyc` & `slitherin-0.7.0/slitherin/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,30 +1,32 @@
 magic:    0xa70d0d0a
-moddate:  0x8f92f165 (Wed Mar 13 11:48:31 2024 UTC)
-files sz: 2693
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 3292
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 25
+   stacksize : 29
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
       090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d0100640064
       086c0e6d0f5a0f0100640064096c106d115a1101006400640a6c126d135a
       1301006400640b6c146d155a1501006400640c6c166d175a170100640064
       0d6c186d195a1901006400640e6c1a6d1b5a1b01006400640f6c1c6d1d5a
       1d0100640064106c1e6d1f5a1f0100640064116c206d215a210100640064
       126c226d235a230100640064136c246d255a250100640064146c266d275a
       270100640064156c286d295a290100640064166c2a6d2b5a2b0100640064
       176c2c6d2d5a2d0100640064186c2e6d2f5a2f0100640064196c306d315a
-      3101006400641a6c326d335a330100652f653167025a3465346503650d65
-      0f6511650b6507650965056513651565176519651b651d651f6521652365
-      25652765016529652b652d653367187a0000005a3567005a36641b84005a
-      37641c5300
+      3101006400641a6c326d335a3301006400641b6c346d355a350100640064
+      1c6c366d375a3701006400641d6c386d395a3901006400641e6c3a6d3b5a
+      3b01006400641f6c3c6d3d5a3d0100652f6531653367035a3e653e650365
+      0d650f6511650b6507650965056513651565176519651b651d651f652165
+      236525652765016529652b652d653565376539653b653d671c7a0000005a
+      3f67005a40642084005a4164215300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('ArbitraryCall',))
                  6 IMPORT_NAME              0 (slitherin.detectors.arbitrary_call.arbitrary_call)
                  8 IMPORT_FROM              1 (ArbitraryCall)
                 10 STORE_NAME               1 (ArbitraryCall)
@@ -195,89 +197,134 @@
                292 LOAD_CONST              25 (('ArbitrumBlockNumberTimestamp',))
                294 IMPORT_NAME             48 (slitherin.detectors.arbitrum.block_number_timestamp)
                296 IMPORT_FROM             49 (ArbitrumBlockNumberTimestamp)
                298 STORE_NAME              49 (ArbitrumBlockNumberTimestamp)
                300 POP_TOP
    
     32         302 LOAD_CONST               0 (0)
-               304 LOAD_CONST              26 (('PotentialArithmOverflow',))
-               306 IMPORT_NAME             50 (slitherin.detectors.potential_arith_overflow)
-               308 IMPORT_FROM             51 (PotentialArithmOverflow)
-               310 STORE_NAME              51 (PotentialArithmOverflow)
+               304 LOAD_CONST              26 (('ArbitrumChainlinkPriceFeed',))
+               306 IMPORT_NAME             50 (slitherin.detectors.arbitrum.arbitrum_chainlink_price_feed)
+               308 IMPORT_FROM             51 (ArbitrumChainlinkPriceFeed)
+               310 STORE_NAME              51 (ArbitrumChainlinkPriceFeed)
                312 POP_TOP
    
-    35         314 LOAD_NAME               47 (ArbitrumPrevrandaoDifficulty)
+    33         314 LOAD_CONST               0 (0)
+               316 LOAD_CONST              27 (('PotentialArithmOverflow',))
+               318 IMPORT_NAME             52 (slitherin.detectors.potential_arith_overflow)
+               320 IMPORT_FROM             53 (PotentialArithmOverflow)
+               322 STORE_NAME              53 (PotentialArithmOverflow)
+               324 POP_TOP
    
-    36         316 LOAD_NAME               49 (ArbitrumBlockNumberTimestamp)
+    34         326 LOAD_CONST               0 (0)
+               328 LOAD_CONST              28 (('CurveReadonlyReentrancy',))
+               330 IMPORT_NAME             54 (slitherin.detectors.curve.curve_readonly_reentrancy)
+               332 IMPORT_FROM             55 (CurveReadonlyReentrancy)
+               334 STORE_NAME              55 (CurveReadonlyReentrancy)
+               336 POP_TOP
    
-    34         318 BUILD_LIST               2
-               320 STORE_NAME              52 (artbitrum_detectors)
+    35         338 LOAD_CONST               0 (0)
+               340 LOAD_CONST              29 (('BalancerReadonlyReentrancy',))
+               342 IMPORT_NAME             56 (slitherin.detectors.balancer.balancer_readonly_reentrancy)
+               344 IMPORT_FROM             57 (BalancerReadonlyReentrancy)
+               346 STORE_NAME              57 (BalancerReadonlyReentrancy)
+               348 POP_TOP
    
-    39         322 LOAD_NAME               52 (artbitrum_detectors)
+    36         350 LOAD_CONST               0 (0)
+               352 LOAD_CONST              30 (('CurveVyperReentrancy',))
+               354 IMPORT_NAME             58 (slitherin.detectors.vyper.reentrancy_curve_vyper_version)
+               356 IMPORT_FROM             59 (CurveVyperReentrancy)
+               358 STORE_NAME              59 (CurveVyperReentrancy)
+               360 POP_TOP
    
-    40         324 LOAD_NAME                3 (DoubleEntryTokenPossiblity)
+    37         362 LOAD_CONST               0 (0)
+               364 LOAD_CONST              31 (('PriceManipulationDetector',))
+               366 IMPORT_NAME             60 (slitherin.detectors.price_manipulation)
+               368 IMPORT_FROM             61 (PriceManipulationDetector)
+               370 STORE_NAME              61 (PriceManipulationDetector)
+               372 POP_TOP
    
-    41         326 LOAD_NAME               13 (UnprotectedSetter)
+    40         374 LOAD_NAME               47 (ArbitrumPrevrandaoDifficulty)
    
-    42         328 LOAD_NAME               15 (NftApproveWarning)
+    41         376 LOAD_NAME               49 (ArbitrumBlockNumberTimestamp)
    
-    43         330 LOAD_NAME               17 (InconsistentNonreentrant)
+    42         378 LOAD_NAME               51 (ArbitrumChainlinkPriceFeed)
    
-    44         332 LOAD_NAME               11 (StrangeSetter)
+    39         380 BUILD_LIST               3
+               382 STORE_NAME              62 (artbitrum_detectors)
    
-    45         334 LOAD_NAME                7 (OnlyEOACheck)
+    45         384 LOAD_NAME               62 (artbitrum_detectors)
    
-    46         336 LOAD_NAME                9 (MagicNumber)
+    46         386 LOAD_NAME                3 (DoubleEntryTokenPossiblity)
    
-    47         338 LOAD_NAME                5 (DubiousTypecast)
+    47         388 LOAD_NAME               13 (UnprotectedSetter)
    
-    48         340 LOAD_NAME               19 (CallForwardToProtected)
+    48         390 LOAD_NAME               15 (NftApproveWarning)
    
-    49         342 LOAD_NAME               21 (MultipleStorageRead)
+    49         392 LOAD_NAME               17 (InconsistentNonreentrant)
    
-    50         344 LOAD_NAME               23 (TimelockController)
+    50         394 LOAD_NAME               11 (StrangeSetter)
    
-    51         346 LOAD_NAME               25 (TxGaspriceWarning)
+    51         396 LOAD_NAME                7 (OnlyEOACheck)
    
-    52         348 LOAD_NAME               27 (UnprotectedInitialize)
+    52         398 LOAD_NAME                9 (MagicNumber)
    
-    53         350 LOAD_NAME               29 (ReadOnlyReentrancy)
+    53         400 LOAD_NAME                5 (DubiousTypecast)
    
-    54         352 LOAD_NAME               31 (EventSetter)
+    54         402 LOAD_NAME               19 (CallForwardToProtected)
    
-    55         354 LOAD_NAME               33 (BeforeTokenTransfer)
+    55         404 LOAD_NAME               21 (MultipleStorageRead)
    
-    56         356 LOAD_NAME               35 (UniswapV2)
+    56         406 LOAD_NAME               23 (TimelockController)
    
-    57         358 LOAD_NAME               37 (TokenFallback)
+    57         408 LOAD_NAME               25 (TxGaspriceWarning)
    
-    58         360 LOAD_NAME               39 (ForContinueIncrement)
+    58         410 LOAD_NAME               27 (UnprotectedInitialize)
    
-    59         362 LOAD_NAME                1 (ArbitraryCall)
+    59         412 LOAD_NAME               29 (ReadOnlyReentrancy)
    
-    60         364 LOAD_NAME               41 (Ecrecover)
+    60         414 LOAD_NAME               31 (EventSetter)
    
-    61         366 LOAD_NAME               43 (PublicVsExternal)
+    61         416 LOAD_NAME               33 (BeforeTokenTransfer)
    
-    62         368 LOAD_NAME               45 (AAVEFlashloanCallbackDetector)
+    62         418 LOAD_NAME               35 (UniswapV2)
    
-    63         370 LOAD_NAME               51 (PotentialArithmOverflow)
+    63         420 LOAD_NAME               37 (TokenFallback)
    
-    39         372 BUILD_LIST              24
-               374 BINARY_OP                0 (+)
-               378 STORE_NAME              53 (plugin_detectors)
+    64         422 LOAD_NAME               39 (ForContinueIncrement)
    
-    65         380 BUILD_LIST               0
-               382 STORE_NAME              54 (plugin_printers)
+    65         424 LOAD_NAME                1 (ArbitraryCall)
    
-    68         384 LOAD_CONST              27 (<code object make_plugin, file "/Users/ndkirillov/Applications/slitherin/slitherin/__init__.py", line 68>)
-               386 MAKE_FUNCTION            0
-               388 STORE_NAME              55 (make_plugin)
-               390 LOAD_CONST              28 (None)
-               392 RETURN_VALUE
+    66         426 LOAD_NAME               41 (Ecrecover)
+   
+    67         428 LOAD_NAME               43 (PublicVsExternal)
+   
+    68         430 LOAD_NAME               45 (AAVEFlashloanCallbackDetector)
+   
+    69         432 LOAD_NAME               53 (PotentialArithmOverflow)
+   
+    70         434 LOAD_NAME               55 (CurveReadonlyReentrancy)
+   
+    71         436 LOAD_NAME               57 (BalancerReadonlyReentrancy)
+   
+    72         438 LOAD_NAME               59 (CurveVyperReentrancy)
+   
+    73         440 LOAD_NAME               61 (PriceManipulationDetector)
+   
+    45         442 BUILD_LIST              28
+               444 BINARY_OP                0 (+)
+               448 STORE_NAME              63 (plugin_detectors)
+   
+    75         450 BUILD_LIST               0
+               452 STORE_NAME              64 (plugin_printers)
+   
+    78         454 LOAD_CONST              32 (<code object make_plugin, file "/Users/ndkirillov/Applications/slitherin/slitherin/__init__.py", line 78>)
+               456 MAKE_FUNCTION            0
+               458 STORE_NAME              65 (make_plugin)
+               460 LOAD_CONST              33 (None)
+               462 RETURN_VALUE
    consts
       0
       ('ArbitraryCall',)
       ('DoubleEntryTokenPossiblity',)
       ('DubiousTypecast',)
       ('OnlyEOACheck',)
       ('MagicNumber',)
@@ -297,45 +344,51 @@
       ('TokenFallback',)
       ('ForContinueIncrement',)
       ('Ecrecover',)
       ('PublicVsExternal',)
       ('AAVEFlashloanCallbackDetector',)
       ('ArbitrumPrevrandaoDifficulty',)
       ('ArbitrumBlockNumberTimestamp',)
+      ('ArbitrumChainlinkPriceFeed',)
       ('PotentialArithmOverflow',)
+      ('CurveReadonlyReentrancy',)
+      ('BalancerReadonlyReentrancy',)
+      ('CurveVyperReentrancy',)
+      ('PriceManipulationDetector',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x9700740000000000000000000000740200000000000000000000660253
             00
-          68           0 RESUME                   0
+          78           0 RESUME                   0
          
-          69           2 LOAD_GLOBAL              0 (plugin_detectors)
+          79           2 LOAD_GLOBAL              0 (plugin_detectors)
                       14 LOAD_GLOBAL              2 (plugin_printers)
                       26 BUILD_TUPLE              2
                       28 RETURN_VALUE
          consts
             None
          names      ('plugin_detectors', 'plugin_printers')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/ndkirillov/Applications/slitherin/slitherin/__init__.py'
          name       'make_plugin'
-         firstlineno 68
+         firstlineno 78
          lnotab 0x0201
       None
-   names      ('slitherin.detectors.arbitrary_call.arbitrary_call', 'ArbitraryCall', 'slitherin.detectors.double_entry_token_possibility', 'DoubleEntryTokenPossiblity', 'slitherin.detectors.dubious_typecast', 'DubiousTypecast', 'slitherin.detectors.falsy_only_eoa_modifier', 'OnlyEOACheck', 'slitherin.detectors.magic_number', 'MagicNumber', 'slitherin.detectors.strange_setter', 'StrangeSetter', 'slitherin.detectors.unprotected_setter', 'UnprotectedSetter', 'slitherin.detectors.nft_approve_warning', 'NftApproveWarning', 'slitherin.detectors.inconsistent_nonreentrant', 'InconsistentNonreentrant', 'slitherin.detectors.call_forward_to_protected', 'CallForwardToProtected', 'slitherin.detectors.multiple_storage_read', 'MultipleStorageRead', 'slitherin.detectors.timelock_controller', 'TimelockController', 'slitherin.detectors.tx_gasprice_warning', 'TxGaspriceWarning', 'slitherin.detectors.unprotected_initialize', 'UnprotectedInitialize', 'slitherin.detectors.read_only_reentrancy', 'ReadOnlyReentrancy', 'slitherin.detectors.event_setter', 'EventSetter', 'slitherin.detectors.before_token_transfer', 'BeforeTokenTransfer', 'slitherin.detectors.uni_v2', 'UniswapV2', 'slitherin.detectors.token_fallback', 'TokenFallback', 'slitherin.detectors.for_continue_increment', 'ForContinueIncrement', 'slitherin.detectors.ecrecover', 'Ecrecover', 'slitherin.detectors.public_vs_external', 'PublicVsExternal', 'slitherin.detectors.aave.flashloan_callback', 'AAVEFlashloanCallbackDetector', 'slitherin.detectors.arbitrum.arbitrum_prevrandao_difficulty', 'ArbitrumPrevrandaoDifficulty', 'slitherin.detectors.arbitrum.block_number_timestamp', 'ArbitrumBlockNumberTimestamp', 'slitherin.detectors.potential_arith_overflow', 'PotentialArithmOverflow', 'artbitrum_detectors', 'plugin_detectors', 'plugin_printers', 'make_plugin')
+   names      ('slitherin.detectors.arbitrary_call.arbitrary_call', 'ArbitraryCall', 'slitherin.detectors.double_entry_token_possibility', 'DoubleEntryTokenPossiblity', 'slitherin.detectors.dubious_typecast', 'DubiousTypecast', 'slitherin.detectors.falsy_only_eoa_modifier', 'OnlyEOACheck', 'slitherin.detectors.magic_number', 'MagicNumber', 'slitherin.detectors.strange_setter', 'StrangeSetter', 'slitherin.detectors.unprotected_setter', 'UnprotectedSetter', 'slitherin.detectors.nft_approve_warning', 'NftApproveWarning', 'slitherin.detectors.inconsistent_nonreentrant', 'InconsistentNonreentrant', 'slitherin.detectors.call_forward_to_protected', 'CallForwardToProtected', 'slitherin.detectors.multiple_storage_read', 'MultipleStorageRead', 'slitherin.detectors.timelock_controller', 'TimelockController', 'slitherin.detectors.tx_gasprice_warning', 'TxGaspriceWarning', 'slitherin.detectors.unprotected_initialize', 'UnprotectedInitialize', 'slitherin.detectors.read_only_reentrancy', 'ReadOnlyReentrancy', 'slitherin.detectors.event_setter', 'EventSetter', 'slitherin.detectors.before_token_transfer', 'BeforeTokenTransfer', 'slitherin.detectors.uni_v2', 'UniswapV2', 'slitherin.detectors.token_fallback', 'TokenFallback', 'slitherin.detectors.for_continue_increment', 'ForContinueIncrement', 'slitherin.detectors.ecrecover', 'Ecrecover', 'slitherin.detectors.public_vs_external', 'PublicVsExternal', 'slitherin.detectors.aave.flashloan_callback', 'AAVEFlashloanCallbackDetector', 'slitherin.detectors.arbitrum.arbitrum_prevrandao_difficulty', 'ArbitrumPrevrandaoDifficulty', 'slitherin.detectors.arbitrum.block_number_timestamp', 'ArbitrumBlockNumberTimestamp', 'slitherin.detectors.arbitrum.arbitrum_chainlink_price_feed', 'ArbitrumChainlinkPriceFeed', 'slitherin.detectors.potential_arith_overflow', 'PotentialArithmOverflow', 'slitherin.detectors.curve.curve_readonly_reentrancy', 'CurveReadonlyReentrancy', 'slitherin.detectors.balancer.balancer_readonly_reentrancy', 'BalancerReadonlyReentrancy', 'slitherin.detectors.vyper.reentrancy_curve_vyper_version', 'CurveVyperReentrancy', 'slitherin.detectors.price_manipulation', 'PriceManipulationDetector', 'artbitrum_detectors', 'plugin_detectors', 'plugin_printers', 'make_plugin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c030c010c010c010c010c010c010c010c010c010c010c
-      010c010c010c010c010c010c010c010c010c010c010c030c030c03020102
-      fe0405020102010201020102010201020102010201020102010201020102
-      01020102010201020102010201020102010201020102e8081a0403
+      010c010c010c010c010c010c010c010c010c010c010c030c030c010c010c
+      010c010c010c030201020102fd0406020102010201020102010201020102
+      010201020102010201020102010201020102010201020102010201020102
+      010201020102010201020102e4081e0403
```

### Comparing `slitherin-0.6.1/slitherin/__pycache__/cli.cpython-311.pyc` & `slitherin-0.7.0/slitherin/__pycache__/cli.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 5232
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/cli.py` & `slitherin-0.7.0/slitherin/cli.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/before_token_transfer.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/before_token_transfer.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 1888
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/call_forward_to_protected.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/call_forward_to_protected.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3980
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/double_entry_token_possibility.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/double_entry_token_possibility.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2045
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/dubious_typecast.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/dubious_typecast.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3915
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/ecrecover.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/ecrecover.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 4239
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/event_setter.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/event_setter.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 1877
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/falsy_only_eoa_modifier.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/falsy_only_eoa_modifier.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5af17165 (Thu Dec  7 16:22:50 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2401
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/for_continue_increment.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/for_continue_increment.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 4677
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/inconsistent_nonreentrant.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/inconsistent_nonreentrant.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3051
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/magic_number.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/magic_number.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3182
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/multiple_storage_read.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/multiple_storage_read.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2522
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/nft_approve_warning.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/nft_approve_warning.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
-files sz: 3110
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 3730
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a086d095a09010064
-      0064056c0a6d0b5a0b0100020047006406840064076501a6030000ab0300
-      000000000000005a0c64085300
+      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d010064075a0e020047
+      006408840064096501a6030000ab0300000000000000005a0f640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AbstractDetector', 'DetectorClassification'))
                  6 IMPORT_NAME              0 (slither.detectors.abstract_detector)
                  8 IMPORT_FROM              1 (AbstractDetector)
                 10 STORE_NAME               1 (AbstractDetector)
@@ -42,124 +42,147 @@
                 48 IMPORT_FROM              8 (Function)
                 50 STORE_NAME               8 (Function)
                 52 IMPORT_FROM              9 (SolidityVariableComposed)
                 54 STORE_NAME               9 (SolidityVariableComposed)
                 56 POP_TOP
    
      5          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('is_dependent',))
-                62 IMPORT_NAME             10 (slither.analyses.data_dependency.data_dependency)
-                64 IMPORT_FROM             11 (is_dependent)
-                66 STORE_NAME              11 (is_dependent)
+                60 LOAD_CONST               5 (('FunctionContract',))
+                62 IMPORT_NAME             10 (slither.core.declarations.function_contract)
+                64 IMPORT_FROM             11 (FunctionContract)
+                66 STORE_NAME              11 (FunctionContract)
                 68 POP_TOP
    
-     8          70 PUSH_NULL
-                72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               6 (<code object NftApproveWarning, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 8>)
-                76 MAKE_FUNCTION            0
-                78 LOAD_CONST               7 ('NftApproveWarning')
-                80 LOAD_NAME                1 (AbstractDetector)
-                82 PRECALL                  3
-                86 CALL                     3
-                96 STORE_NAME              12 (NftApproveWarning)
-                98 LOAD_CONST               8 (None)
-               100 RETURN_VALUE
+     6          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('is_dependent',))
+                74 IMPORT_NAME             12 (slither.analyses.data_dependency.data_dependency)
+                76 IMPORT_FROM             13 (is_dependent)
+                78 STORE_NAME              13 (is_dependent)
+                80 POP_TOP
+   
+     8          82 LOAD_CONST               7 ('safeTransferFrom(address,address,address,uint256)')
+                84 STORE_NAME              14 (SAFE_ERC20_LIB_SIG)
+   
+     9          86 PUSH_NULL
+                88 LOAD_BUILD_CLASS
+                90 LOAD_CONST               8 (<code object NftApproveWarning, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 9>)
+                92 MAKE_FUNCTION            0
+                94 LOAD_CONST               9 ('NftApproveWarning')
+                96 LOAD_NAME                1 (AbstractDetector)
+                98 PRECALL                  3
+               102 CALL                     3
+               112 STORE_NAME              15 (NftApproveWarning)
+               114 LOAD_CONST              10 (None)
+               116 RETURN_VALUE
    consts
       0
       ('AbstractDetector', 'DetectorClassification')
       ('List',)
       ('Node',)
       ('Function', 'SolidityVariableComposed')
+      ('FunctionContract',)
       ('is_dependent',)
+      'safeTransferFrom(address,address,address,uint256)'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0565066a07000000
             00000000005a0865066a0900000000000000005a0a64045a0b64055a0c64
-            065a0d64075a0e64085a0f67006409a2015a10640a65116602640b84045a
-            12640c65136514190000000000000000006602640d84045a15640e84005a
-            16640f5300
-           8           0 RESUME                   0
+            065a0d64075a0e64085a0f6409640a640b6510640c640d67065a11640e65
+            126602640f84045a13641065146515190000000000000000006602641184
+            045a16641284005a1764135300
+           9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('NftApproveWarning')
                        8 STORE_NAME               2 (__qualname__)
          
-           9          10 LOAD_CONST               1 ('\n    Sees if contract contains erc721.[safe]TransferFrom(from, ...) where from parameter is not related to msg.sender\n    ')
+          10          10 LOAD_CONST               1 ('\n    Sees if contract contains erc721.[safe]TransferFrom(from, ...) where from parameter is not related to msg.sender\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          13          14 LOAD_CONST               2 ('pess-nft-approve-warning')
+          14          14 LOAD_CONST               2 ('pess-nft-approve-warning')
                       16 STORE_NAME               4 (ARGUMENT)
          
-          14          18 LOAD_CONST               3 ('[safe]TransferFrom(from,...) - from parameter is not related to msg.sender')
+          15          18 LOAD_CONST               3 ('[safe]TransferFrom(from,...) - from parameter is not related to msg.sender')
                       20 STORE_NAME               5 (HELP)
          
-          15          22 LOAD_NAME                6 (DetectorClassification)
+          16          22 LOAD_NAME                6 (DetectorClassification)
                       24 LOAD_ATTR                7 (MEDIUM)
                       34 STORE_NAME               8 (IMPACT)
          
-          16          36 LOAD_NAME                6 (DetectorClassification)
+          17          36 LOAD_NAME                6 (DetectorClassification)
                       38 LOAD_ATTR                9 (LOW)
                       48 STORE_NAME              10 (CONFIDENCE)
          
-          18          50 LOAD_CONST               4 ('https://ventral.digital/posts/2022/8/18/sznsdaos-bountyboard-unauthorized-transferfrom-vulnerability')
+          19          50 LOAD_CONST               4 ('https://ventral.digital/posts/2022/8/18/sznsdaos-bountyboard-unauthorized-transferfrom-vulnerability')
                       52 STORE_NAME              11 (WIKI)
          
-          19          54 LOAD_CONST               5 ('NFT Approve Warning')
+          20          54 LOAD_CONST               5 ('Token Approve Warning')
                       56 STORE_NAME              12 (WIKI_TITLE)
          
-          20          58 LOAD_CONST               6 ('In [safe]TransferFrom() from parameter must be related to msg.sender')
+          21          58 LOAD_CONST               6 ('In [safe]TransferFrom() from parameter must be related to msg.sender')
                       60 STORE_NAME              13 (WIKI_DESCRIPTION)
          
-          21          62 LOAD_CONST               7 ('-')
+          22          62 LOAD_CONST               7 ('-')
                       64 STORE_NAME              14 (WIKI_EXPLOIT_SCENARIO)
          
-          22          66 LOAD_CONST               8 ('from parameter must be related to msg.sender')
+          23          66 LOAD_CONST               8 ('from parameter must be related to msg.sender')
                       68 STORE_NAME              15 (WIKI_RECOMMENDATION)
          
-          24          70 BUILD_LIST               0
-                      72 LOAD_CONST               9 (('transferFrom(address,address,uint256)', 'safeTransferFrom(address,address,uint256,bytes)', 'safeTransferFrom(address,address,uint256)'))
-                      74 LIST_EXTEND              1
-                      76 STORE_NAME              16 (_signatures)
-         
-          26          78 LOAD_CONST              10 ('f')
-                      80 LOAD_NAME               17 (Function)
-                      82 BUILD_TUPLE              2
-                      84 LOAD_CONST              11 (<code object _detect_arbitrary_from, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 26>)
-                      86 MAKE_FUNCTION            4 (annotations)
-                      88 STORE_NAME              18 (_detect_arbitrary_from)
-         
-          41          90 LOAD_CONST              12 ('nodes')
-                      92 LOAD_NAME               19 (List)
-                      94 LOAD_NAME               20 (Node)
-                      96 BINARY_SUBSCR
-                     106 BUILD_TUPLE              2
-                     108 LOAD_CONST              13 (<code object _arbitrary_from, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 41>)
-                     110 MAKE_FUNCTION            4 (annotations)
-                     112 STORE_NAME              21 (_arbitrary_from)
-         
-          58         114 LOAD_CONST              14 (<code object _detect, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 58>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              22 (_detect)
-                     120 LOAD_CONST              15 (None)
-                     122 RETURN_VALUE
+          25          70 LOAD_CONST               9 ('transferFrom(address,address,uint256)')
+                      72 LOAD_CONST              10 ('safeTransferFrom(address,address,uint256,bytes)')
+                      74 LOAD_CONST              11 ('safeTransferFrom(address,address,uint256)')
+         
+          26          76 LOAD_NAME               16 (SAFE_ERC20_LIB_SIG)
+         
+          27          78 LOAD_CONST              12 ('safeTransferFrom(address,address,uint256,uint256,bytes)')
+                      80 LOAD_CONST              13 ('safeBatchTransferFrom(address,address,uint256[],uint256[],bytes)')
+         
+          25          82 BUILD_LIST               6
+                      84 STORE_NAME              17 (_signatures)
+         
+          29          86 LOAD_CONST              14 ('f')
+                      88 LOAD_NAME               18 (Function)
+                      90 BUILD_TUPLE              2
+                      92 LOAD_CONST              15 (<code object _detect_arbitrary_from, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 29>)
+                      94 MAKE_FUNCTION            4 (annotations)
+                      96 STORE_NAME              19 (_detect_arbitrary_from)
+         
+          44          98 LOAD_CONST              16 ('nodes')
+                     100 LOAD_NAME               20 (List)
+                     102 LOAD_NAME               21 (Node)
+                     104 BINARY_SUBSCR
+                     114 BUILD_TUPLE              2
+                     116 LOAD_CONST              17 (<code object _arbitrary_from, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 44>)
+                     118 MAKE_FUNCTION            4 (annotations)
+                     120 STORE_NAME              22 (_arbitrary_from)
+         
+          62         122 LOAD_CONST              18 (<code object _detect, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 62>)
+                     124 MAKE_FUNCTION            0
+                     126 STORE_NAME              23 (_detect)
+                     128 LOAD_CONST              19 (None)
+                     130 RETURN_VALUE
          consts
             'NftApproveWarning'
             '\n    Sees if contract contains erc721.[safe]TransferFrom(from, ...) where from parameter is not related to msg.sender\n    '
             'pess-nft-approve-warning'
             '[safe]TransferFrom(from,...) - from parameter is not related to msg.sender'
             'https://ventral.digital/posts/2022/8/18/sznsdaos-bountyboard-unauthorized-transferfrom-vulnerability'
-            'NFT Approve Warning'
+            'Token Approve Warning'
             'In [safe]TransferFrom() from parameter must be related to msg.sender'
             '-'
             'from parameter must be related to msg.sender'
-            ('transferFrom(address,address,uint256)', 'safeTransferFrom(address,address,uint256,bytes)', 'safeTransferFrom(address,address,uint256)')
+            'transferFrom(address,address,uint256)'
+            'safeTransferFrom(address,address,uint256,bytes)'
+            'safeTransferFrom(address,address,uint256)'
+            'safeTransferFrom(address,address,uint256,uint256,bytes)'
+            'safeBatchTransferFrom(address,address,uint256[],uint256[],bytes)'
             'f'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
@@ -169,121 +192,121 @@
                   000000000074070000000000000000000088046601640384087c006a0400
                   00000000000000a6020000ab020000000000000000a6010000ab01000000
                   0000000000721a7c00a00500000000000000000000000000000000000000
                   007c016a060000000000000000a6010000ab010000000000000000530067
                   005300
                              0 MAKE_CELL                4 (all_calls)
                
-                26           2 RESUME                   0
+                29           2 RESUME                   0
                
-                27           4 LOAD_CONST               1 (<code object <listcomp>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 27>)
+                30           4 LOAD_CONST               1 (<code object <listcomp>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 30>)
                              6 MAKE_FUNCTION            0
                
-                29           8 LOAD_FAST                1 (f)
+                32           8 LOAD_FAST                1 (f)
                             10 LOAD_ATTR                0 (high_level_calls)
                
-                27          20 GET_ITER
+                30          20 GET_ITER
                             22 PRECALL                  0
                             26 CALL                     0
                             36 STORE_FAST               2 (all_high_level_calls)
                
-                32          38 LOAD_CONST               2 (<code object <listcomp>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 32>)
+                35          38 LOAD_CONST               2 (<code object <listcomp>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 35>)
                             40 MAKE_FUNCTION            0
                             42 LOAD_FAST                1 (f)
                             44 LOAD_ATTR                1 (library_calls)
                             54 GET_ITER
                             56 PRECALL                  0
                             60 CALL                     0
                             70 STORE_FAST               3 (all_library_calls)
                
-                34          72 LOAD_FAST                2 (all_high_level_calls)
+                37          72 LOAD_FAST                2 (all_high_level_calls)
                             74 LOAD_FAST                3 (all_library_calls)
                             76 BINARY_OP                0 (+)
                             80 STORE_DEREF              4 (all_calls)
                
-                36          82 LOAD_GLOBAL              5 (NULL + any)
+                39          82 LOAD_GLOBAL              5 (NULL + any)
                             94 LOAD_GLOBAL              7 (NULL + map)
                            106 LOAD_CLOSURE             4 (all_calls)
                            108 BUILD_TUPLE              1
-                           110 LOAD_CONST               3 (<code object <lambda>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 36>)
+                           110 LOAD_CONST               3 (<code object <lambda>, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py", line 39>)
                            112 MAKE_FUNCTION            8 (closure)
                            114 LOAD_FAST                0 (self)
                            116 LOAD_ATTR                4 (_signatures)
                            126 PRECALL                  2
                            130 CALL                     2
                            140 PRECALL                  1
                            144 CALL                     1
                            154 POP_JUMP_FORWARD_IF_FALSE    26 (to 208)
                
-                37         156 LOAD_FAST                0 (self)
+                40         156 LOAD_FAST                0 (self)
                            158 LOAD_METHOD              5 (_arbitrary_from)
                            180 LOAD_FAST                1 (f)
                            182 LOAD_ATTR                6 (nodes)
                            192 PRECALL                  1
                            196 CALL                     1
                            206 RETURN_VALUE
                
-                39     >>  208 BUILD_LIST               0
+                42     >>  208 BUILD_LIST               0
                            210 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d2a7d017401000000000000000000007c016400190000
                         00000000000000740200000000000000000000a6020000ab020000000000
                         000000af1d7c016400190000000000000000006a02000000000000000091
                         028c2b5300
-                      27           0 RESUME                   0
+                      30           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                42 (to 92)
                      
-                      29           8 STORE_FAST               1 (f_called)
+                      32           8 STORE_FAST               1 (f_called)
                      
-                      30          10 LOAD_GLOBAL              1 (NULL + isinstance)
+                      33          10 LOAD_GLOBAL              1 (NULL + isinstance)
                                   22 LOAD_FAST                1 (f_called)
                                   24 LOAD_CONST               0 (1)
                                   26 BINARY_SUBSCR
                                   36 LOAD_GLOBAL              2 (Function)
                                   48 PRECALL                  2
                                   52 CALL                     2
                      
-                      27          62 POP_JUMP_BACKWARD_IF_FALSE    29 (to 6)
+                      30          62 POP_JUMP_BACKWARD_IF_FALSE    29 (to 6)
                      
-                      28          64 LOAD_FAST                1 (f_called)
+                      31          64 LOAD_FAST                1 (f_called)
                                   66 LOAD_CONST               0 (1)
                                   68 BINARY_SUBSCR
                                   78 LOAD_ATTR                2 (solidity_signature)
                      
-                      27          88 LIST_APPEND              2
+                      30          88 LIST_APPEND              2
                                   90 JUMP_BACKWARD           43 (to 6)
                              >>   92 RETURN_VALUE
                      consts
                         1
                      names      ('isinstance', 'Function', 'solidity_signature')
                      varnames   ('.0', 'f_called')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                      name       '<listcomp>'
-                     firstlineno 27
+                     firstlineno 30
                      lnotab 0x0802020134fd020118ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0f7d017c016400190000000000000000006a00000000
                         000000000091028c105300
-                      32           0 RESUME                   0
+                      35           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                15 (to 38)
                                    8 STORE_FAST               1 (f_called)
                                   10 LOAD_FAST                1 (f_called)
                                   12 LOAD_CONST               0 (1)
                                   14 BINARY_SUBSCR
@@ -295,194 +318,232 @@
                         1
                      names      ('solidity_signature',)
                      varnames   ('.0', 'f_called')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                      name       '<listcomp>'
-                     firstlineno 32
+                     firstlineno 35
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code 0x950197007c00890176005300
                                    0 COPY_FREE_VARS           1
                      
-                      36           2 RESUME                   0
+                      39           2 RESUME                   0
                                    4 LOAD_FAST                0 (s)
                                    6 LOAD_DEREF               1 (all_calls)
                                    8 CONTAINS_OP              0
                                   10 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('s',)
                      freevars   ('all_calls',)
                      cellvars   ()
                      filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                      name       '<lambda>'
-                     firstlineno 36
+                     firstlineno 39
                      lnotab 0x
                names      ('high_level_calls', 'library_calls', 'any', 'map', '_signatures', '_arbitrary_from', 'nodes')
                varnames   ('self', 'f', 'all_high_level_calls', 'all_library_calls')
                freevars   ()
                cellvars   ('all_calls',)
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                name       '_detect_arbitrary_from'
-               firstlineno 26
+               firstlineno 29
                lnotab 0x040104020cfe120522020a024a013402
             'nodes'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 8
                flags     : 3
                code
-                  0x970067007d027c0144005d937d037c036a00000000000000000044005d
-                  897d047403000000000000000000007c046401a6020000ab020000000000
-                  00000072777403000000000000000000007c046a02000000000000000064
-                  02a6020000ab02000000000000000072627c046a0200000000000000006a
-                  0300000000000000007c006a0400000000000000007600724f740b000000
-                  000000000000007c046a0600000000000000006403190000000000000000
-                  00740f000000000000000000006404a6010000ab0100000000000000007c
-                  036a0200000000000000006a080000000000000000a6030000ab03000000
-                  00000000007d057c05731a7c02a009000000000000000000000000000000
-                  00000000007c046a0a0000000000000000a6010000ab0100000000000000
-                  0001008c8a8c947c025300
-                41           0 RESUME                   0
+                  0x970067007d027c0144005df07d037c036a00000000000000000044005d
+                  e67d047403000000000000000000007c046401a6020000ab020000000000
+                  00000072d47403000000000000000000007c046a02000000000000000064
+                  02a6020000ab02000000000000000072bf7c046a0200000000000000006a
+                  0300000000000000007c006a040000000000000000760072ac7c046a0200
+                  000000000000006a030000000000000000740a000000000000000000006b
+                  03000000007233740d000000000000000000007c046a0700000000000000
+                  006403190000000000000000007411000000000000000000006404a60100
+                  00ab0100000000000000007c036a0200000000000000006a090000000000
+                  000000a6030000ab03000000000000000070477c046a0200000000000000
+                  006a030000000000000000740a000000000000000000006b02000000006f
+                  32740d000000000000000000007c046a0700000000000000006405190000
+                  000000000000007411000000000000000000006404a6010000ab01000000
+                  00000000007c036a0200000000000000006a090000000000000000a60300
+                  00ab0300000000000000007d057c05731a7c02a00a000000000000000000
+                  00000000000000000000007c046a0b0000000000000000a6010000ab0100
+                  0000000000000001008ce78cf17c025300
+                44           0 RESUME                   0
                
-                43           2 BUILD_LIST               0
+                46           2 BUILD_LIST               0
                              4 STORE_FAST               2 (irList)
                
-                44           6 LOAD_FAST                1 (nodes)
+                47           6 LOAD_FAST                1 (nodes)
                              8 GET_ITER
-                       >>   10 FOR_ITER               147 (to 306)
+                       >>   10 FOR_ITER               240 (to 492)
                             12 STORE_FAST               3 (node)
                
-                45          14 LOAD_FAST                3 (node)
+                48          14 LOAD_FAST                3 (node)
                             16 LOAD_ATTR                0 (irs)
                             26 GET_ITER
-                       >>   28 FOR_ITER               137 (to 304)
+                       >>   28 FOR_ITER               230 (to 490)
                             30 STORE_FAST               4 (ir)
                
-                47          32 LOAD_GLOBAL              3 (NULL + hasattr)
+                50          32 LOAD_GLOBAL              3 (NULL + hasattr)
                             44 LOAD_FAST                4 (ir)
                             46 LOAD_CONST               1 ('function')
                             48 PRECALL                  2
                             52 CALL                     2
                
-                46          62 POP_JUMP_FORWARD_IF_FALSE   119 (to 302)
+                49          62 POP_JUMP_FORWARD_IF_FALSE   212 (to 488)
                
-                48          64 LOAD_GLOBAL              3 (NULL + hasattr)
+                51          64 LOAD_GLOBAL              3 (NULL + hasattr)
                             76 LOAD_FAST                4 (ir)
                             78 LOAD_ATTR                2 (function)
                             88 LOAD_CONST               2 ('solidity_signature')
                             90 PRECALL                  2
                             94 CALL                     2
                
-                46         104 POP_JUMP_FORWARD_IF_FALSE    98 (to 302)
+                49         104 POP_JUMP_FORWARD_IF_FALSE   191 (to 488)
                
-                49         106 LOAD_FAST                4 (ir)
+                52         106 LOAD_FAST                4 (ir)
                            108 LOAD_ATTR                2 (function)
                            118 LOAD_ATTR                3 (solidity_signature)
                            128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                4 (_signatures)
                            140 CONTAINS_OP              0
-                           142 POP_JUMP_FORWARD_IF_FALSE    79 (to 302)
+                           142 POP_JUMP_FORWARD_IF_FALSE   172 (to 488)
                
-                51         144 LOAD_GLOBAL             11 (NULL + is_dependent)
-                           156 LOAD_FAST                4 (ir)
-                           158 LOAD_ATTR                6 (arguments)
-                           168 LOAD_CONST               3 (0)
-                           170 BINARY_SUBSCR
-                           180 LOAD_GLOBAL             15 (NULL + SolidityVariableComposed)
-                           192 LOAD_CONST               4 ('msg.sender')
-                           194 PRECALL                  1
-                           198 CALL                     1
-                           208 LOAD_FAST                3 (node)
-                           210 LOAD_ATTR                2 (function)
-                           220 LOAD_ATTR                8 (contract)
-                           230 PRECALL                  3
-                           234 CALL                     3
-                           244 STORE_FAST               5 (is_from_sender)
-               
-                53         246 LOAD_FAST                5 (is_from_sender)
-                           248 POP_JUMP_FORWARD_IF_TRUE    26 (to 302)
-               
-                54         250 LOAD_FAST                2 (irList)
-                           252 LOAD_METHOD              9 (append)
-                           274 LOAD_FAST                4 (ir)
-                           276 LOAD_ATTR               10 (node)
-                           286 PRECALL                  1
-                           290 CALL                     1
-                           300 POP_TOP
-                       >>  302 JUMP_BACKWARD          138 (to 28)
+                54         144 LOAD_FAST                4 (ir)
+                           146 LOAD_ATTR                2 (function)
+                           156 LOAD_ATTR                3 (solidity_signature)
+                           166 LOAD_GLOBAL             10 (SAFE_ERC20_LIB_SIG)
+                           178 COMPARE_OP               3 (!=)
+                           184 POP_JUMP_FORWARD_IF_FALSE    51 (to 288)
+                           186 LOAD_GLOBAL             13 (NULL + is_dependent)
+                           198 LOAD_FAST                4 (ir)
+                           200 LOAD_ATTR                7 (arguments)
+                           210 LOAD_CONST               3 (0)
+                           212 BINARY_SUBSCR
+                           222 LOAD_GLOBAL             17 (NULL + SolidityVariableComposed)
+                           234 LOAD_CONST               4 ('msg.sender')
+                           236 PRECALL                  1
+                           240 CALL                     1
+                           250 LOAD_FAST                3 (node)
+                           252 LOAD_ATTR                2 (function)
+                           262 LOAD_ATTR                9 (contract)
+                           272 PRECALL                  3
+                           276 CALL                     3
+                           286 JUMP_IF_TRUE_OR_POP     71 (to 430)
+               
+                55     >>  288 LOAD_FAST                4 (ir)
+                           290 LOAD_ATTR                2 (function)
+                           300 LOAD_ATTR                3 (solidity_signature)
+                           310 LOAD_GLOBAL             10 (SAFE_ERC20_LIB_SIG)
+                           322 COMPARE_OP               2 (==)
+                           328 JUMP_IF_FALSE_OR_POP    50 (to 430)
+                           330 LOAD_GLOBAL             13 (NULL + is_dependent)
+                           342 LOAD_FAST                4 (ir)
+                           344 LOAD_ATTR                7 (arguments)
+                           354 LOAD_CONST               5 (1)
+                           356 BINARY_SUBSCR
+                           366 LOAD_GLOBAL             17 (NULL + SolidityVariableComposed)
+                           378 LOAD_CONST               4 ('msg.sender')
+                           380 PRECALL                  1
+                           384 CALL                     1
+                           394 LOAD_FAST                3 (node)
+                           396 LOAD_ATTR                2 (function)
+                           406 LOAD_ATTR                9 (contract)
+                           416 PRECALL                  3
+                           420 CALL                     3
+               
+                54     >>  430 STORE_FAST               5 (is_from_sender)
+               
+                57         432 LOAD_FAST                5 (is_from_sender)
+                           434 POP_JUMP_FORWARD_IF_TRUE    26 (to 488)
+               
+                58         436 LOAD_FAST                2 (irList)
+                           438 LOAD_METHOD             10 (append)
+                           460 LOAD_FAST                4 (ir)
+                           462 LOAD_ATTR               11 (node)
+                           472 PRECALL                  1
+                           476 CALL                     1
+                           486 POP_TOP
+                       >>  488 JUMP_BACKWARD          231 (to 28)
                
-                45     >>  304 JUMP_BACKWARD          148 (to 10)
+                48     >>  490 JUMP_BACKWARD          241 (to 10)
                
-                55     >>  306 LOAD_FAST                2 (irList)
-                           308 RETURN_VALUE
+                59     >>  492 LOAD_FAST                2 (irList)
+                           494 RETURN_VALUE
                consts
                   'Finds instances of (safe)transferFrom that do not use msg.sender or address(this) as from parameter.'
                   'function'
                   'solidity_signature'
                   0
                   'msg.sender'
-               names      ('irs', 'hasattr', 'function', 'solidity_signature', '_signatures', 'is_dependent', 'arguments', 'SolidityVariableComposed', 'contract', 'append', 'node')
+                  1
+               names      ('irs', 'hasattr', 'function', 'solidity_signature', '_signatures', 'SAFE_ERC20_LIB_SIG', 'is_dependent', 'arguments', 'SolidityVariableComposed', 'contract', 'append', 'node')
                varnames   ('self', 'nodes', 'irList', 'node', 'ir', 'is_from_sender')
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                name       '_arbitrary_from'
-               firstlineno 41
-               lnotab 0x02020401080112021eff020228fe020326026602040136f7020a
+               firstlineno 44
+               lnotab
+                  0x02020401080112021eff020228fe0203260290018eff0203040136f602
+                  0b
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 13
                flags     : 3
                code
                   0x970067007d017c006a0000000000000000006a01000000000000000044
                   005d617d027c026a02000000000000000044005d577d037c00a003000000
                   00000000000000000000000000000000007c03a6010000ab010000000000
                   00000044005d3f7d047c01a0040000000000000000000000000000000000
                   0000007c00a00500000000000000000000000000000000000000007c036a
                   0600000000000000006a07000000000000000064017c036a070000000000
                   00000064027c0464036706a6010000ab010000000000000000a6010000ab
                   01000000000000000001008c408c588c627c015300
-                58           0 RESUME                   0
+                62           0 RESUME                   0
                
-                60           2 BUILD_LIST               0
+                64           2 BUILD_LIST               0
                              4 STORE_FAST               1 (res)
                
-                61           6 LOAD_FAST                0 (self)
+                65           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (compilation_unit)
                             18 LOAD_ATTR                1 (contracts_derived)
                             28 GET_ITER
                        >>   30 FOR_ITER                97 (to 226)
                             32 STORE_FAST               2 (c)
                
-                62          34 LOAD_FAST                2 (c)
+                66          34 LOAD_FAST                2 (c)
                             36 LOAD_ATTR                2 (functions)
                             46 GET_ITER
                        >>   48 FOR_ITER                87 (to 224)
                             50 STORE_FAST               3 (f)
                
-                63          52 LOAD_FAST                0 (self)
+                67          52 LOAD_FAST                0 (self)
                             54 LOAD_METHOD              3 (_detect_arbitrary_from)
                             76 LOAD_FAST                3 (f)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 GET_ITER
                        >>   94 FOR_ITER                63 (to 222)
                             96 STORE_FAST               4 (d)
                
-                64          98 LOAD_FAST                1 (res)
+                68          98 LOAD_FAST                1 (res)
                            100 LOAD_METHOD              4 (append)
                            122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD              5 (generate_result)
                            146 LOAD_FAST                3 (f)
                            148 LOAD_ATTR                6 (contract_declarer)
                            158 LOAD_ATTR                7 (name)
                            168 LOAD_CONST               1 (' ')
@@ -495,45 +556,47 @@
                            190 PRECALL                  1
                            194 CALL                     1
                            204 PRECALL                  1
                            208 CALL                     1
                            218 POP_TOP
                            220 JUMP_BACKWARD           64 (to 94)
                
-                63     >>  222 JUMP_BACKWARD           88 (to 48)
+                67     >>  222 JUMP_BACKWARD           88 (to 48)
                
-                62     >>  224 JUMP_BACKWARD           98 (to 30)
+                66     >>  224 JUMP_BACKWARD           98 (to 30)
                
-                65     >>  226 LOAD_FAST                1 (res)
+                69     >>  226 LOAD_FAST                1 (res)
                            228 RETURN_VALUE
                consts
                   'Detect transfers that use arbitrary `from` parameter.'
                   ' '
                   ' parameter from is not related to msg.sender '
                   '\n'
                names      ('compilation_unit', 'contracts_derived', 'functions', '_detect_arbitrary_from', 'append', 'generate_result', 'contract_declarer', 'name')
                varnames   ('self', 'res', 'c', 'f', 'd')
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
                name       '_detect'
-               firstlineno 58
+               firstlineno 62
                lnotab 0x020204011c0112012e017cff02ff0203
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ARGUMENT', 'HELP', 'DetectorClassification', 'MEDIUM', 'IMPACT', 'LOW', 'CONFIDENCE', 'WIKI', 'WIKI_TITLE', 'WIKI_DESCRIPTION', 'WIKI_EXPLOIT_SCENARIO', 'WIKI_RECOMMENDATION', '_signatures', 'Function', '_detect_arbitrary_from', 'List', 'Node', '_arbitrary_from', '_detect')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ARGUMENT', 'HELP', 'DetectorClassification', 'MEDIUM', 'IMPACT', 'LOW', 'CONFIDENCE', 'WIKI', 'WIKI_TITLE', 'WIKI_DESCRIPTION', 'WIKI_EXPLOIT_SCENARIO', 'WIKI_RECOMMENDATION', 'SAFE_ERC20_LIB_SIG', '_signatures', 'Function', '_detect_arbitrary_from', 'List', 'Node', '_arbitrary_from', '_detect')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
          name       'NftApproveWarning'
-         firstlineno 8
-         lnotab 0x0a010404040104010e010e020401040104010401040208020c0f1811
+         firstlineno 9
+         lnotab
+            0x0a010404040104010e010e02040104010401040104020601020104fe04
+            040c0f1812
       'NftApproveWarning'
       None
-   names      ('slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'typing', 'List', 'slither.core.cfg.node', 'Node', 'slither.core.declarations', 'Function', 'SolidityVariableComposed', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'NftApproveWarning')
+   names      ('slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'typing', 'List', 'slither.core.cfg.node', 'Node', 'slither.core.declarations', 'Function', 'SolidityVariableComposed', 'slither.core.declarations.function_contract', 'FunctionContract', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'SAFE_ERC20_LIB_SIG', 'NftApproveWarning')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/nft_approve_warning.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020110010c010c0110010c03
+   lnotab 0x00ff020110010c010c0110010c010c020401
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/potential_arith_overflow.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/potential_arith_overflow.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
-files sz: 7621
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 7652
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -579,22 +579,22 @@
             'fun'
             code
                argcount  : 2
                nlocals   : 14
                stacksize : 8
                flags     : 3
                code
-                  0x970067007d0264017d037c016a000000000000000000440090025dd87d
+                  0x970067007d0264017d037c016a000000000000000000440090025de07d
                   047c046a0100000000000000007404000000000000000000006a03000000
                   00000000007500720364027d036e157c046a010000000000000000740400
                   0000000000000000006a0400000000000000007500720264017d037c046a
                   0100000000000000007404000000000000000000006a0500000000000000
                   00750073277c046a0100000000000000007404000000000000000000006a
                   060000000000000000750073147c046a0100000000000000007404000000
-                  000000000000006a0700000000000000007500900272707c039002736d7c
+                  000000000000006a0700000000000000007500900272787c03900273757c
                   046a0800000000000000007d057413000000000000000000007c05a60100
                   00ab01000000000000000064036b04000000009001721a74150000000000
                   00000000007c056404190000000000000000007416000000000000000000
                   006a0c0000000000000000a6020000ab02000000000000000072fa741b00
                   0000000000000000007c056404190000000000000000006a0e0000000000
                   0000006a0f0000000000000000a6010000ab010000000000000000742000
                   000000000000000000760072d4741b000000000000000000007c05640419
@@ -608,48 +608,49 @@
                   00000000007c0a7c07a6020000ab0200000000000000005c0300007d0b7d
                   0c7d0d7c087c0b7a1400007d087c09a01400000000000000000000000000
                   000000000000007c0ca6010000ab01000000000000000001008c377c0872
                   357c02a01500000000000000000000000000000000000000007c04741b00
                   0000000000000000007c056404190000000000000000006a0e0000000000
                   0000006a0f0000000000000000a6010000ab0100000000000000007c0966
                   03a6010000ab01000000000000000001007413000000000000000000007c
-                  05a6010000ab01000000000000000064036b040000000090017224741500
+                  05a6010000ab01000000000000000064036b04000000009001722c741500
                   0000000000000000007c0564041900000000000000000074160000000000
                   00000000006a160000000000000000a6020000ab02000000000000000090
-                  0172037413000000000000000000007c016a170000000000000000a60100
-                  00ab01000000000000000064086b020000000072eb741b00000000000000
-                  0000007c016a170000000000000000640319000000000000000000a60100
-                  00ab010000000000000000742000000000000000000000760072ca741b00
-                  0000000000000000007c016a170000000000000000640319000000000000
-                  000000a6010000ab010000000000000000a0110000000000000000000000
-                  0000000000000000006405a6010000ab010000000000000000a011000000
-                  00000000000000000000000000000000006406a6010000ab010000000000
-                  0000007d067425000000000000000000007c06730264076e017c06a60100
-                  00ab0100000000000000007d0764017d0867007d097c0564006404850219
-                  00000000000000000044005d367d0a7c00a0130000000000000000000000
-                  0000000000000000007c0a7c07a6020000ab0200000000000000005c0300
-                  007d0b7d0c7d0d7c087c0b7a1400007d087c09a014000000000000000000
-                  00000000000000000000007c0ca6010000ab01000000000000000001008c
-                  377c0872307c02a01500000000000000000000000000000000000000007c
-                  04741b000000000000000000007c016a1700000000000000006403190000
-                  00000000000000a6010000ab0100000000000000007c096603a6010000ab
-                  010000000000000000010090028cda7c025300
+                  01720b7c016a170000000000000000900181037413000000000000000000
+                  007c016a170000000000000000a6010000ab01000000000000000064086b
+                  020000000072eb741b000000000000000000007c016a1700000000000000
+                  00640319000000000000000000a6010000ab010000000000000000742000
+                  000000000000000000760072ca741b000000000000000000007c016a1700
+                  00000000000000640319000000000000000000a6010000ab010000000000
+                  000000a01100000000000000000000000000000000000000006405a60100
+                  00ab010000000000000000a0110000000000000000000000000000000000
+                  0000006406a6010000ab0100000000000000007d06742500000000000000
+                  0000007c06730264076e017c06a6010000ab0100000000000000007d0764
+                  017d0867007d097c056400640485021900000000000000000044005d367d
+                  0a7c00a01300000000000000000000000000000000000000007c0a7c07a6
+                  020000ab0200000000000000005c0300007d0b7d0c7d0d7c087c0b7a1400
+                  007d087c09a01400000000000000000000000000000000000000007c0ca6
+                  010000ab01000000000000000001008c377c0872307c02a0150000000000
+                  0000000000000000000000000000007c04741b000000000000000000007c
+                  016a170000000000000000640319000000000000000000a6010000ab0100
+                  000000000000007c096603a6010000ab010000000000000000010090028c
+                  e27c025300
                 68           0 RESUME                   0
                
                 69           2 BUILD_LIST               0
                              4 STORE_FAST               2 (final_results)
                
                 70           6 LOAD_CONST               1 (False)
                              8 STORE_FAST               3 (is_active_assembly)
                
                 71          10 LOAD_FAST                1 (fun)
                             12 LOAD_ATTR                0 (nodes)
                             22 GET_ITER
                        >>   24 EXTENDED_ARG             2
-                            26 FOR_ITER               728 (to 1484)
+                            26 FOR_ITER               736 (to 1500)
                             28 STORE_FAST               4 (node)
                
                 72          30 LOAD_FAST                4 (node)
                             32 LOAD_ATTR                1 (type)
                             42 LOAD_GLOBAL              4 (NodeType)
                             54 LOAD_ATTR                3 (ASSEMBLY)
                             64 IS_OP                    0
@@ -683,18 +684,18 @@
                            190 POP_JUMP_FORWARD_IF_TRUE    20 (to 232)
                            192 LOAD_FAST                4 (node)
                            194 LOAD_ATTR                1 (type)
                            204 LOAD_GLOBAL              4 (NodeType)
                            216 LOAD_ATTR                7 (RETURN)
                            226 IS_OP                    0
                            228 EXTENDED_ARG             2
-                           230 POP_JUMP_FORWARD_IF_FALSE   624 (to 1480)
+                           230 POP_JUMP_FORWARD_IF_FALSE   632 (to 1496)
                        >>  232 LOAD_FAST                3 (is_active_assembly)
                            234 EXTENDED_ARG             2
-                           236 POP_JUMP_FORWARD_IF_TRUE   621 (to 1480)
+                           236 POP_JUMP_FORWARD_IF_TRUE   629 (to 1496)
                
                 77         238 LOAD_FAST                4 (node)
                            240 LOAD_ATTR                8 (irs)
                            250 STORE_FAST               5 (irs)
                
                 78         252 LOAD_GLOBAL             19 (NULL + len)
                            264 LOAD_FAST                5 (irs)
@@ -815,133 +816,137 @@
                 89     >>  856 LOAD_GLOBAL             19 (NULL + len)
                            868 LOAD_FAST                5 (irs)
                            870 PRECALL                  1
                            874 CALL                     1
                            884 LOAD_CONST               3 (0)
                            886 COMPARE_OP               4 (>)
                            892 EXTENDED_ARG             1
-                           894 POP_JUMP_FORWARD_IF_FALSE   292 (to 1480)
+                           894 POP_JUMP_FORWARD_IF_FALSE   300 (to 1496)
                            896 LOAD_GLOBAL             21 (NULL + isinstance)
                            908 LOAD_FAST                5 (irs)
                            910 LOAD_CONST               4 (-1)
                            912 BINARY_SUBSCR
                            922 LOAD_GLOBAL             22 (ops)
                            934 LOAD_ATTR               22 (Return)
                            944 PRECALL                  2
                            948 CALL                     2
                            958 EXTENDED_ARG             1
-                           960 POP_JUMP_FORWARD_IF_FALSE   259 (to 1480)
-                           962 LOAD_GLOBAL             19 (NULL + len)
-                           974 LOAD_FAST                1 (fun)
-                           976 LOAD_ATTR               23 (return_type)
-                           986 PRECALL                  1
-                           990 CALL                     1
-                          1000 LOAD_CONST               8 (1)
-                          1002 COMPARE_OP               2 (==)
-                          1008 POP_JUMP_FORWARD_IF_FALSE   235 (to 1480)
-                          1010 LOAD_GLOBAL             27 (NULL + str)
-                          1022 LOAD_FAST                1 (fun)
-                          1024 LOAD_ATTR               23 (return_type)
-                          1034 LOAD_CONST               3 (0)
-                          1036 BINARY_SUBSCR
-                          1046 PRECALL                  1
-                          1050 CALL                     1
-                          1060 LOAD_GLOBAL             32 (INT_TYPES)
-                          1072 CONTAINS_OP              0
-                          1074 POP_JUMP_FORWARD_IF_FALSE   202 (to 1480)
-               
-                90        1076 LOAD_GLOBAL             27 (NULL + str)
-                          1088 LOAD_FAST                1 (fun)
-                          1090 LOAD_ATTR               23 (return_type)
-                          1100 LOAD_CONST               3 (0)
-                          1102 BINARY_SUBSCR
-                          1112 PRECALL                  1
-                          1116 CALL                     1
-                          1126 LOAD_METHOD             17 (removeprefix)
-                          1148 LOAD_CONST               5 ('uint')
-                          1150 PRECALL                  1
-                          1154 CALL                     1
-                          1164 LOAD_METHOD             17 (removeprefix)
-                          1186 LOAD_CONST               6 ('int')
-                          1188 PRECALL                  1
-                          1192 CALL                     1
-                          1202 STORE_FAST               6 (expected_bits_cut)
-               
-                91        1204 LOAD_GLOBAL             37 (NULL + int)
-                          1216 LOAD_FAST                6 (expected_bits_cut)
-                          1218 POP_JUMP_FORWARD_IF_TRUE     2 (to 1224)
-                          1220 LOAD_CONST               7 (256)
-                          1222 JUMP_FORWARD             1 (to 1226)
-                       >> 1224 LOAD_FAST                6 (expected_bits_cut)
-                       >> 1226 PRECALL                  1
-                          1230 CALL                     1
-                          1240 STORE_FAST               7 (expected_bits)
-               
-                92        1242 LOAD_CONST               1 (False)
-                          1244 STORE_FAST               8 (has_problems)
-               
-                93        1246 BUILD_LIST               0
-                          1248 STORE_FAST               9 (errors)
-               
-                94        1250 LOAD_FAST                5 (irs)
-                          1252 LOAD_CONST               0 (None)
-                          1254 LOAD_CONST               4 (-1)
-                          1256 BUILD_SLICE              2
-                          1258 BINARY_SUBSCR
-                          1268 GET_ITER
-                       >> 1270 FOR_ITER                54 (to 1380)
-                          1272 STORE_FAST              10 (x)
-               
-                95        1274 LOAD_FAST                0 (self)
-                          1276 LOAD_METHOD             19 (_has_op_overflowing_sub_expression)
-                          1298 LOAD_FAST               10 (x)
-                          1300 LOAD_FAST                7 (expected_bits)
-                          1302 PRECALL                  2
-                          1306 CALL                     2
-                          1316 UNPACK_SEQUENCE          3
-                          1320 STORE_FAST              11 (response_res)
-                          1322 STORE_FAST              12 (response_errors)
-                          1324 STORE_FAST              13 (_)
-               
-                96        1326 LOAD_FAST                8 (has_problems)
-                          1328 LOAD_FAST               11 (response_res)
-                          1330 BINARY_OP               20 (|=)
-                          1334 STORE_FAST               8 (has_problems)
-               
-                97        1336 LOAD_FAST                9 (errors)
-                          1338 LOAD_METHOD             20 (extend)
-                          1360 LOAD_FAST               12 (response_errors)
-                          1362 PRECALL                  1
-                          1366 CALL                     1
-                          1376 POP_TOP
-                          1378 JUMP_BACKWARD           55 (to 1270)
-               
-                98     >> 1380 LOAD_FAST                8 (has_problems)
-                          1382 POP_JUMP_FORWARD_IF_FALSE    48 (to 1480)
-               
-                99        1384 LOAD_FAST                2 (final_results)
-                          1386 LOAD_METHOD             21 (append)
-                          1408 LOAD_FAST                4 (node)
-                          1410 LOAD_GLOBAL             27 (NULL + str)
-                          1422 LOAD_FAST                1 (fun)
-                          1424 LOAD_ATTR               23 (return_type)
-                          1434 LOAD_CONST               3 (0)
-                          1436 BINARY_SUBSCR
-                          1446 PRECALL                  1
-                          1450 CALL                     1
-                          1460 LOAD_FAST                9 (errors)
-                          1462 BUILD_TUPLE              3
-                          1464 PRECALL                  1
-                          1468 CALL                     1
-                          1478 POP_TOP
-                       >> 1480 EXTENDED_ARG             2
-                          1482 JUMP_BACKWARD          730 (to 24)
+                           960 POP_JUMP_FORWARD_IF_FALSE   267 (to 1496)
+                           962 LOAD_FAST                1 (fun)
+                           964 LOAD_ATTR               23 (return_type)
+                           974 EXTENDED_ARG             1
+                           976 POP_JUMP_FORWARD_IF_NONE   259 (to 1496)
+                           978 LOAD_GLOBAL             19 (NULL + len)
+                           990 LOAD_FAST                1 (fun)
+                           992 LOAD_ATTR               23 (return_type)
+                          1002 PRECALL                  1
+                          1006 CALL                     1
+                          1016 LOAD_CONST               8 (1)
+                          1018 COMPARE_OP               2 (==)
+                          1024 POP_JUMP_FORWARD_IF_FALSE   235 (to 1496)
+                          1026 LOAD_GLOBAL             27 (NULL + str)
+                          1038 LOAD_FAST                1 (fun)
+                          1040 LOAD_ATTR               23 (return_type)
+                          1050 LOAD_CONST               3 (0)
+                          1052 BINARY_SUBSCR
+                          1062 PRECALL                  1
+                          1066 CALL                     1
+                          1076 LOAD_GLOBAL             32 (INT_TYPES)
+                          1088 CONTAINS_OP              0
+                          1090 POP_JUMP_FORWARD_IF_FALSE   202 (to 1496)
+               
+                90        1092 LOAD_GLOBAL             27 (NULL + str)
+                          1104 LOAD_FAST                1 (fun)
+                          1106 LOAD_ATTR               23 (return_type)
+                          1116 LOAD_CONST               3 (0)
+                          1118 BINARY_SUBSCR
+                          1128 PRECALL                  1
+                          1132 CALL                     1
+                          1142 LOAD_METHOD             17 (removeprefix)
+                          1164 LOAD_CONST               5 ('uint')
+                          1166 PRECALL                  1
+                          1170 CALL                     1
+                          1180 LOAD_METHOD             17 (removeprefix)
+                          1202 LOAD_CONST               6 ('int')
+                          1204 PRECALL                  1
+                          1208 CALL                     1
+                          1218 STORE_FAST               6 (expected_bits_cut)
+               
+                91        1220 LOAD_GLOBAL             37 (NULL + int)
+                          1232 LOAD_FAST                6 (expected_bits_cut)
+                          1234 POP_JUMP_FORWARD_IF_TRUE     2 (to 1240)
+                          1236 LOAD_CONST               7 (256)
+                          1238 JUMP_FORWARD             1 (to 1242)
+                       >> 1240 LOAD_FAST                6 (expected_bits_cut)
+                       >> 1242 PRECALL                  1
+                          1246 CALL                     1
+                          1256 STORE_FAST               7 (expected_bits)
+               
+                92        1258 LOAD_CONST               1 (False)
+                          1260 STORE_FAST               8 (has_problems)
+               
+                93        1262 BUILD_LIST               0
+                          1264 STORE_FAST               9 (errors)
+               
+                94        1266 LOAD_FAST                5 (irs)
+                          1268 LOAD_CONST               0 (None)
+                          1270 LOAD_CONST               4 (-1)
+                          1272 BUILD_SLICE              2
+                          1274 BINARY_SUBSCR
+                          1284 GET_ITER
+                       >> 1286 FOR_ITER                54 (to 1396)
+                          1288 STORE_FAST              10 (x)
+               
+                95        1290 LOAD_FAST                0 (self)
+                          1292 LOAD_METHOD             19 (_has_op_overflowing_sub_expression)
+                          1314 LOAD_FAST               10 (x)
+                          1316 LOAD_FAST                7 (expected_bits)
+                          1318 PRECALL                  2
+                          1322 CALL                     2
+                          1332 UNPACK_SEQUENCE          3
+                          1336 STORE_FAST              11 (response_res)
+                          1338 STORE_FAST              12 (response_errors)
+                          1340 STORE_FAST              13 (_)
+               
+                96        1342 LOAD_FAST                8 (has_problems)
+                          1344 LOAD_FAST               11 (response_res)
+                          1346 BINARY_OP               20 (|=)
+                          1350 STORE_FAST               8 (has_problems)
+               
+                97        1352 LOAD_FAST                9 (errors)
+                          1354 LOAD_METHOD             20 (extend)
+                          1376 LOAD_FAST               12 (response_errors)
+                          1378 PRECALL                  1
+                          1382 CALL                     1
+                          1392 POP_TOP
+                          1394 JUMP_BACKWARD           55 (to 1286)
+               
+                98     >> 1396 LOAD_FAST                8 (has_problems)
+                          1398 POP_JUMP_FORWARD_IF_FALSE    48 (to 1496)
+               
+                99        1400 LOAD_FAST                2 (final_results)
+                          1402 LOAD_METHOD             21 (append)
+                          1424 LOAD_FAST                4 (node)
+                          1426 LOAD_GLOBAL             27 (NULL + str)
+                          1438 LOAD_FAST                1 (fun)
+                          1440 LOAD_ATTR               23 (return_type)
+                          1450 LOAD_CONST               3 (0)
+                          1452 BINARY_SUBSCR
+                          1462 PRECALL                  1
+                          1466 CALL                     1
+                          1476 LOAD_FAST                9 (errors)
+                          1478 BUILD_TUPLE              3
+                          1480 PRECALL                  1
+                          1484 CALL                     1
+                          1494 POP_TOP
+                       >> 1496 EXTENDED_ARG             2
+                          1498 JUMP_BACKWARD          738 (to 24)
                
-               101     >> 1484 LOAD_FAST                2 (final_results)
-                          1486 RETURN_VALUE
+               101     >> 1500 LOAD_FAST                2 (final_results)
+                          1502 RETURN_VALUE
                consts
                   None
                   False
                   True
                   0
                   -1
                   'uint'
@@ -953,15 +958,15 @@
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/potential_arith_overflow.py'
                name       '_find_vulnerable_expressions'
                firstlineno 68
                lnotab
                   0x020104010401140126010601260104017a010e01b4018a012601040104
-                  01180134010a012c0104016a01dc018001260104010401180134010a012c
+                  01180134010a012c0104016a01ec018001260104010401180134010a012c
                   0104016402
             code
                argcount  : 1
                nlocals   : 11
                stacksize : 12
                flags     : 3
                code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/public_vs_external.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/public_vs_external.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2117
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/read_only_reentrancy.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/read_only_reentrancy.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,26 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
-files sz: 17933
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 17952
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a030100640164036c046d
       055a056d065a066d075a070100640164046c086d095a090100640164056c
       0a6d0b5a0b0100640164066c0c6d0d5a0d6d0e5a0e6d0f5a0f0100640164
-      076c106d115a110100640864096c126d135a136d145a146d155a156d165a
-      166d175a176d185a1801006401640a6c196d1a5a1a010002006502640b64
-      0c640d6702a6020000ab0200000000000000005a1b02006502640e670064
-      0fa201a6020000ab0200000000000000005a1c6410650f6411650f641265
-      1d6606641384045a1e020047006414840064156515a6030000ab03000000
-      00000000005a1f020047006416840064176513a6030000ab030000000000
-      0000005a2064185300
+      076c106d115a110100640164086c126d135a136d145a146d155a156d165a
+      166d175a176d185a180100640164096c196d1a5a1a010002006502640a64
+      0b640c6702a6020000ab0200000000000000005a1b02006502640d670064
+      0ea201a6020000ab0200000000000000005a1c640f650f6410650f641165
+      1d6606641284045a1e020047006413840064146515a6030000ab03000000
+      00000000005a1f020047006415840064166513a6030000ab030000000000
+      0000005a2064175300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('"\n    Re-entrancy detection\n    Based on heuristics, it may lead to FP and FN\n    Iterate over all the nodes of the graph until reaching a fixpoint\n')
                  4 STORE_NAME               0 (__doc__)
    
      6           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('namedtuple', 'defaultdict'))
@@ -70,17 +70,17 @@
     11          86 LOAD_CONST               1 (0)
                 88 LOAD_CONST               7 (('DetectorClassification',))
                 90 IMPORT_NAME             16 (slither.detectors.abstract_detector)
                 92 IMPORT_FROM             17 (DetectorClassification)
                 94 STORE_NAME              17 (DetectorClassification)
                 96 POP_TOP
    
-    12          98 LOAD_CONST               8 (1)
-               100 LOAD_CONST               9 (('Reentrancy', 'to_hashable', 'AbstractState', 'union_dict', '_filter_if', 'is_subset'))
-               102 IMPORT_NAME             18 (reentrancy.reentrancy)
+    12          98 LOAD_CONST               1 (0)
+               100 LOAD_CONST               8 (('Reentrancy', 'to_hashable', 'AbstractState', 'union_dict', '_filter_if', 'is_subset'))
+               102 IMPORT_NAME             18 (slitherin.detectors.reentrancy.reentrancy)
                104 IMPORT_FROM             19 (Reentrancy)
                106 STORE_NAME              19 (Reentrancy)
                108 IMPORT_FROM             20 (to_hashable)
                110 STORE_NAME              20 (to_hashable)
                112 IMPORT_FROM             21 (AbstractState)
                114 STORE_NAME              21 (AbstractState)
                116 IMPORT_FROM             22 (union_dict)
@@ -88,82 +88,81 @@
                120 IMPORT_FROM             23 (_filter_if)
                122 STORE_NAME              23 (_filter_if)
                124 IMPORT_FROM             24 (is_subset)
                126 STORE_NAME              24 (is_subset)
                128 POP_TOP
    
     20         130 LOAD_CONST               1 (0)
-               132 LOAD_CONST              10 (('EventCall',))
+               132 LOAD_CONST               9 (('EventCall',))
                134 IMPORT_NAME             25 (slither.slithir.operations)
                136 IMPORT_FROM             26 (EventCall)
                138 STORE_NAME              26 (EventCall)
                140 POP_TOP
    
     22         142 PUSH_NULL
                144 LOAD_NAME                2 (namedtuple)
-               146 LOAD_CONST              11 ('FindingKey')
-               148 LOAD_CONST              12 ('function')
-               150 LOAD_CONST              13 ('calls')
+               146 LOAD_CONST              10 ('FindingKey')
+               148 LOAD_CONST              11 ('function')
+               150 LOAD_CONST              12 ('calls')
                152 BUILD_LIST               2
                154 PRECALL                  2
                158 CALL                     2
                168 STORE_NAME              27 (FindingKey)
    
     23         170 PUSH_NULL
                172 LOAD_NAME                2 (namedtuple)
-               174 LOAD_CONST              14 ('FindingValue')
+               174 LOAD_CONST              13 ('FindingValue')
                176 BUILD_LIST               0
-               178 LOAD_CONST              15 (('variable', 'written_at', 'node', 'nodes'))
+               178 LOAD_CONST              14 (('variable', 'written_at', 'node', 'nodes'))
                180 LIST_EXTEND              1
                182 PRECALL                  2
                186 CALL                     2
                196 STORE_NAME              28 (FindingValue)
    
-    26         198 LOAD_CONST              16 ('a')
+    26         198 LOAD_CONST              15 ('a')
                200 LOAD_NAME               15 (Contract)
-               202 LOAD_CONST              17 ('b')
+               202 LOAD_CONST              16 ('b')
                204 LOAD_NAME               15 (Contract)
-               206 LOAD_CONST              18 ('return')
+               206 LOAD_CONST              17 ('return')
                208 LOAD_NAME               29 (bool)
                210 BUILD_TUPLE              6
-               212 LOAD_CONST              19 (<code object are_same_contract, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 26>)
+               212 LOAD_CONST              18 (<code object are_same_contract, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 26>)
                214 MAKE_FUNCTION            4 (annotations)
                216 STORE_NAME              30 (are_same_contract)
    
     33         218 PUSH_NULL
                220 LOAD_BUILD_CLASS
-               222 LOAD_CONST              20 (<code object ReadOnlyReentrancyState, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 33>)
+               222 LOAD_CONST              19 (<code object ReadOnlyReentrancyState, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 33>)
                224 MAKE_FUNCTION            0
-               226 LOAD_CONST              21 ('ReadOnlyReentrancyState')
+               226 LOAD_CONST              20 ('ReadOnlyReentrancyState')
                228 LOAD_NAME               21 (AbstractState)
                230 PRECALL                  3
                234 CALL                     3
                244 STORE_NAME              31 (ReadOnlyReentrancyState)
    
    173         246 PUSH_NULL
                248 LOAD_BUILD_CLASS
-               250 LOAD_CONST              22 (<code object ReadOnlyReentrancy, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 173>)
+               250 LOAD_CONST              21 (<code object ReadOnlyReentrancy, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py", line 173>)
                252 MAKE_FUNCTION            0
-               254 LOAD_CONST              23 ('ReadOnlyReentrancy')
+               254 LOAD_CONST              22 ('ReadOnlyReentrancy')
                256 LOAD_NAME               19 (Reentrancy)
                258 PRECALL                  3
                262 CALL                     3
                272 STORE_NAME              32 (ReadOnlyReentrancy)
-               274 LOAD_CONST              24 (None)
+               274 LOAD_CONST              23 (None)
                276 RETURN_VALUE
    consts
       '"\n    Re-entrancy detection\n    Based on heuristics, it may lead to FP and FN\n    Iterate over all the nodes of the graph until reaching a fixpoint\n'
       0
       ('namedtuple', 'defaultdict')
       ('Dict', 'List', 'Set')
       ('Variable',)
       ('Function',)
       ('NodeType', 'Node', 'Contract')
       ('DetectorClassification',)
-      1
       ('Reentrancy', 'to_hashable', 'AbstractState', 'union_dict', '_filter_if', 'is_subset')
       ('EventCall',)
       'FindingKey'
       'function'
       'calls'
       'FindingValue'
       ('variable', 'written_at', 'node', 'nodes')
@@ -3012,15 +3011,15 @@
          name       'ReadOnlyReentrancy'
          firstlineno 173
          lnotab
             0x0e01040104010e010e02040104010401040104023c0314fe040112ff12
             040825061c065d0645
       'ReadOnlyReentrancy'
       None
-   names      ('__doc__', 'collections', 'namedtuple', 'defaultdict', 'typing', 'Dict', 'List', 'Set', 'slither.core.variables.variable', 'Variable', 'slither.core.declarations', 'Function', 'slither.core.cfg.node', 'NodeType', 'Node', 'Contract', 'slither.detectors.abstract_detector', 'DetectorClassification', 'reentrancy.reentrancy', 'Reentrancy', 'to_hashable', 'AbstractState', 'union_dict', '_filter_if', 'is_subset', 'slither.slithir.operations', 'EventCall', 'FindingKey', 'FindingValue', 'bool', 'are_same_contract', 'ReadOnlyReentrancyState', 'ReadOnlyReentrancy')
+   names      ('__doc__', 'collections', 'namedtuple', 'defaultdict', 'typing', 'Dict', 'List', 'Set', 'slither.core.variables.variable', 'Variable', 'slither.core.declarations', 'Function', 'slither.core.cfg.node', 'NodeType', 'Node', 'Contract', 'slither.detectors.abstract_detector', 'DetectorClassification', 'slitherin.detectors.reentrancy.reentrancy', 'Reentrancy', 'to_hashable', 'AbstractState', 'union_dict', '_filter_if', 'is_subset', 'slither.slithir.operations', 'EventCall', 'FindingKey', 'FindingValue', 'bool', 'are_same_contract', 'ReadOnlyReentrancyState', 'ReadOnlyReentrancy')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/read_only_reentrancy.py'
    name       '<module>'
    firstlineno 1
    lnotab
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/strange_setter.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/strange_setter.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
-files sz: 4488
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 5201
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a056d065a060100640064046c076d085a080100640064056c
-      096d0a630201006d0b630201006d0c5a0d01000200470064068400640765
-      05a6030000ab0300000000000000005a0e64055300
+      096d0a630201006d0b630201006d0c5a0d0100640064056c0e6d0a630201
+      006d0b630201006d0f5a100100640064066c116d125a1201000200470064
+      07840064086505a6030000ab0300000000000000005a1364055300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('List',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
@@ -52,106 +53,127 @@
                 66 IMPORT_FROM             11 (expressions)
                 68 SWAP                     2
                 70 POP_TOP
                 72 IMPORT_FROM             12 (new_array)
                 74 STORE_NAME              13 (na)
                 76 POP_TOP
    
-     8          78 PUSH_NULL
-                80 LOAD_BUILD_CLASS
-                82 LOAD_CONST               6 (<code object StrangeSetter, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 8>)
-                84 MAKE_FUNCTION            0
-                86 LOAD_CONST               7 ('StrangeSetter')
-                88 LOAD_NAME                5 (AbstractDetector)
-                90 PRECALL                  3
-                94 CALL                     3
-               104 STORE_NAME              14 (StrangeSetter)
-               106 LOAD_CONST               5 (None)
-               108 RETURN_VALUE
+     6          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               5 (None)
+                82 IMPORT_NAME             14 (slither.core.expressions.new_contract)
+                84 IMPORT_FROM             10 (core)
+                86 SWAP                     2
+                88 POP_TOP
+                90 IMPORT_FROM             11 (expressions)
+                92 SWAP                     2
+                94 POP_TOP
+                96 IMPORT_FROM             15 (new_contract)
+                98 STORE_NAME              16 (nc)
+               100 POP_TOP
+   
+     7         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               6 (('is_dependent',))
+               106 IMPORT_NAME             17 (slither.analyses.data_dependency.data_dependency)
+               108 IMPORT_FROM             18 (is_dependent)
+               110 STORE_NAME              18 (is_dependent)
+               112 POP_TOP
+   
+    10         114 PUSH_NULL
+               116 LOAD_BUILD_CLASS
+               118 LOAD_CONST               7 (<code object StrangeSetter, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 10>)
+               120 MAKE_FUNCTION            0
+               122 LOAD_CONST               8 ('StrangeSetter')
+               124 LOAD_NAME                5 (AbstractDetector)
+               126 PRECALL                  3
+               130 CALL                     3
+               140 STORE_NAME              19 (StrangeSetter)
+               142 LOAD_CONST               5 (None)
+               144 RETURN_VALUE
    consts
       0
       ('List',)
       ('Output',)
       ('AbstractDetector', 'DetectorClassification')
       ('Function',)
       None
+      ('is_dependent',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0565066a07000000
             00000000005a0865066a0900000000000000005a0a64045a0b64055a0c64
             065a0d64075a0e64085a0f64096510640a65116604640b84045a12640965
             10640a65116604640c84045a13640a651465151900000000000000000066
             02640d84045a16640e5300
-           8           0 RESUME                   0
+          10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('StrangeSetter')
                        8 STORE_NAME               2 (__qualname__)
          
-           9          10 LOAD_CONST               1 ('\n    Sees if contract contains a setter, that does not change contract storage variables or that does not use arguments for an external call.\n    ')
+          11          10 LOAD_CONST               1 ('\n    Sees if contract contains a setter, that does not change contract storage variables or that does not use arguments for an external call.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          13          14 LOAD_CONST               2 ('pess-strange-setter')
+          15          14 LOAD_CONST               2 ('pess-strange-setter')
                       16 STORE_NAME               4 (ARGUMENT)
          
-          14          18 LOAD_CONST               3 ('Contract storage parameter is not changed by setter')
+          16          18 LOAD_CONST               3 ('Contract storage parameter is not changed by setter')
                       20 STORE_NAME               5 (HELP)
          
-          15          22 LOAD_NAME                6 (DetectorClassification)
+          17          22 LOAD_NAME                6 (DetectorClassification)
                       24 LOAD_ATTR                7 (HIGH)
                       34 STORE_NAME               8 (IMPACT)
          
-          16          36 LOAD_NAME                6 (DetectorClassification)
+          18          36 LOAD_NAME                6 (DetectorClassification)
                       38 LOAD_ATTR                9 (MEDIUM)
                       48 STORE_NAME              10 (CONFIDENCE)
          
-          19          50 LOAD_CONST               4 ('https://github.com/pessimistic-io/slitherin/blob/master/docs/strange_setter.md')
+          21          50 LOAD_CONST               4 ('https://github.com/pessimistic-io/slitherin/blob/master/docs/strange_setter.md')
          
-          18          52 STORE_NAME              11 (WIKI)
+          20          52 STORE_NAME              11 (WIKI)
          
-          21          54 LOAD_CONST               5 ('Strange Setter')
+          23          54 LOAD_CONST               5 ('Strange Setter')
                       56 STORE_NAME              12 (WIKI_TITLE)
          
-          22          58 LOAD_CONST               6 ('Setter must write to storage variables or pass arguments to external calls')
+          24          58 LOAD_CONST               6 ('Setter must write to storage variables or pass arguments to external calls')
                       60 STORE_NAME              13 (WIKI_DESCRIPTION)
          
-          23          62 LOAD_CONST               7 ('-')
+          25          62 LOAD_CONST               7 ('-')
                       64 STORE_NAME              14 (WIKI_EXPLOIT_SCENARIO)
          
-          24          66 LOAD_CONST               8 ('Make sure that your setter actually sets something')
+          26          66 LOAD_CONST               8 ('Make sure that your setter actually sets something')
                       68 STORE_NAME              15 (WIKI_RECOMMENDATION)
          
-          26          70 LOAD_CONST               9 ('fun')
+          28          70 LOAD_CONST               9 ('fun')
                       72 LOAD_NAME               16 (Function)
                       74 LOAD_CONST              10 ('return')
                       76 LOAD_NAME               17 (bool)
                       78 BUILD_TUPLE              4
-                      80 LOAD_CONST              11 (<code object _is_strange_setter, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 26>)
+                      80 LOAD_CONST              11 (<code object _is_strange_setter, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 28>)
                       82 MAKE_FUNCTION            4 (annotations)
                       84 STORE_NAME              18 (_is_strange_setter)
          
-          60          86 LOAD_CONST               9 ('fun')
+          71          86 LOAD_CONST               9 ('fun')
                       88 LOAD_NAME               16 (Function)
                       90 LOAD_CONST              10 ('return')
                       92 LOAD_NAME               17 (bool)
                       94 BUILD_TUPLE              4
-                      96 LOAD_CONST              12 (<code object _is_strange_constructor, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 60>)
+                      96 LOAD_CONST              12 (<code object _is_strange_constructor, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 71>)
                       98 MAKE_FUNCTION            4 (annotations)
                      100 STORE_NAME              19 (_is_strange_constructor)
          
-          64         102 LOAD_CONST              10 ('return')
+          75         102 LOAD_CONST              10 ('return')
                      104 LOAD_NAME               20 (List)
                      106 LOAD_NAME               21 (Output)
                      108 BINARY_SUBSCR
                      118 BUILD_TUPLE              2
-                     120 LOAD_CONST              13 (<code object _detect, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 64>)
+                     120 LOAD_CONST              13 (<code object _detect, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py", line 75>)
                      122 MAKE_FUNCTION            4 (annotations)
                      124 STORE_NAME              22 (_detect)
                      126 LOAD_CONST              14 (None)
                      128 RETURN_VALUE
          consts
             'StrangeSetter'
             '\n    Sees if contract contains a setter, that does not change contract storage variables or that does not use arguments for an external call.\n    '
@@ -162,16 +184,16 @@
             'Setter must write to storage variables or pass arguments to external calls'
             '-'
             'Make sure that your setter actually sets something'
             'fun'
             'return'
             code
                argcount  : 2
-               nlocals   : 9
-               stacksize : 7
+               nlocals   : 12
+               stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000007c01740200000000000000000000a6
                   020000ab0200000000000000007302640153007c016a0200000000000000
                   00730264025300740700000000000000000000a6000000ab000000000000
                   0000007d027c016a04000000000000000044005d657d0374010000000000
                   00000000007c03740200000000000000000000a6020000ab020000000000
@@ -182,259 +204,330 @@
                   000000000000000000000000000000000000007c04a6010000ab01000000
                   000000000001008c3d8c478c667c016a02000000000000000044005d467d
                   047c016a060000000000000000723d7c016a05000000000000000044005d
                   357d05740f000000000000000000007c04a6010000ab0100000000000000
                   00740f000000000000000000007c05a6010000ab01000000000000000076
                   0072157c02a00800000000000000000000000000000000000000007c04a6
                   010000ab01000000000000000001008c368c477c016a0200000000000000
-                  0044005d797d047c016a09000000000000000044005d6f7d067401000000
+                  0044005d997d047c016a09000000000000000044005d8f7d067401000000
                   000000000000007c066a0a00000000000000007416000000000000000000
-                  006a0c0000000000000000a6020000ab02000000000000000072018c2267
-                  007c066a0d0000000000000000a2017c066a0a00000000000000006a0e00
-                  00000000000000910144005d377d07740f000000000000000000007c07a6
-                  010000ab010000000000000000740f000000000000000000007c04a60100
-                  00ab0100000000000000006b020000000072157c02a00800000000000000
-                  000000000000000000000000007c04a6010000ab01000000000000000001
-                  008c388c708c7a741f000000000000000000007407000000000000000000
-                  007c016a020000000000000000a6010000ab0100000000000000007c027a
-                  010000a6010000ab0100000000000000007d087c08741f00000000000000
-                  0000007c016a020000000000000000a6010000ab0100000000000000006b
-                  03000000005300
-                26           0 RESUME                   0
+                  006a0c0000000000000000a6020000ab02000000000000000072018c2274
+                  01000000000000000000007c066a0a0000000000000000741a0000000000
+                  00000000006a0e0000000000000000a6020000ab02000000000000000072
+                  018c4267007c066a0f0000000000000000a2017c066a0a00000000000000
+                  006a100000000000000000910144005d377d07740f000000000000000000
+                  007c07a6010000ab010000000000000000740f000000000000000000007c
+                  04a6010000ab0100000000000000006b020000000072157c02a008000000
+                  00000000000000000000000000000000007c04a6010000ab010000000000
+                  00000001008c388c908c9a7c016a11000000000000000064036b02000000
+                  0072597c016a12000000000000000044005d517d087c00a0130000000000
+                  0000000000000000000000000000007c08a6010000ab0100000000000000
+                  00733a7c016a02000000000000000044005d327d097c086a020000000000
+                  00000044005d287d0a7429000000000000000000007c0a7c097c08a60300
+                  00ab03000000000000000072157c02a00800000000000000000000000000
+                  000000000000007c09a6010000ab01000000000000000001008c298c338c
+                  52742b000000000000000000007407000000000000000000007c016a0200
+                  00000000000000a6010000ab0100000000000000007c027a010000a60100
+                  00ab0100000000000000007d0b7c0b742b000000000000000000007c016a
+                  020000000000000000a6010000ab0100000000000000006b030000000053
+                  00
+                28           0 RESUME                   0
                
-                28           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                30           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (fun)
                             16 LOAD_GLOBAL              2 (Function)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                
-                29          44 LOAD_CONST               1 (True)
+                31          44 LOAD_CONST               1 (True)
                             46 RETURN_VALUE
                
-                31     >>   48 LOAD_FAST                1 (fun)
+                33     >>   48 LOAD_FAST                1 (fun)
                             50 LOAD_ATTR                2 (parameters)
                             60 POP_JUMP_FORWARD_IF_TRUE     2 (to 66)
                
-                33          62 LOAD_CONST               2 (False)
+                35          62 LOAD_CONST               2 (False)
                             64 RETURN_VALUE
                
-                34     >>   66 LOAD_GLOBAL              7 (NULL + set)
+                36     >>   66 LOAD_GLOBAL              7 (NULL + set)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 STORE_FAST               2 (used_params)
                
-                37          94 LOAD_FAST                1 (fun)
+                39          94 LOAD_FAST                1 (fun)
                             96 LOAD_ATTR                4 (internal_calls)
                
-                35         106 GET_ITER
+                37         106 GET_ITER
                        >>  108 FOR_ITER               101 (to 312)
                
-                36         110 STORE_FAST               3 (fin)
+                38         110 STORE_FAST               3 (fin)
                
-                38         112 LOAD_GLOBAL              1 (NULL + isinstance)
+                40         112 LOAD_GLOBAL              1 (NULL + isinstance)
                            124 LOAD_FAST                3 (fin)
                            126 LOAD_GLOBAL              2 (Function)
                            138 PRECALL                  2
                            142 CALL                     2
                            152 POP_JUMP_FORWARD_IF_FALSE    78 (to 310)
                
-                39         154 LOAD_FAST                3 (fin)
+                41         154 LOAD_FAST                3 (fin)
                            156 LOAD_ATTR                2 (parameters)
                            166 GET_ITER
                        >>  168 FOR_ITER                70 (to 310)
                            170 STORE_FAST               4 (param)
                
-                40         172 LOAD_FAST                3 (fin)
+                42         172 LOAD_FAST                3 (fin)
                            174 LOAD_ATTR                5 (nodes)
                            184 GET_ITER
                        >>  186 FOR_ITER                60 (to 308)
                            188 STORE_FAST               5 (n)
                
-                41         190 LOAD_FAST                5 (n)
+                43         190 LOAD_FAST                5 (n)
                            192 LOAD_ATTR                6 (state_variables_written)
                            202 POP_JUMP_FORWARD_IF_FALSE    51 (to 306)
                            204 LOAD_GLOBAL             15 (NULL + str)
                            216 LOAD_FAST                4 (param)
                            218 PRECALL                  1
                            222 CALL                     1
                            232 LOAD_GLOBAL             15 (NULL + str)
                
-                42         244 LOAD_FAST                5 (n)
+                44         244 LOAD_FAST                5 (n)
                
-                41         246 PRECALL                  1
+                43         246 PRECALL                  1
                            250 CALL                     1
                            260 CONTAINS_OP              0
                            262 POP_JUMP_FORWARD_IF_FALSE    21 (to 306)
                
-                44         264 LOAD_FAST                2 (used_params)
+                46         264 LOAD_FAST                2 (used_params)
                            266 LOAD_METHOD              8 (add)
                            288 LOAD_FAST                4 (param)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 POP_TOP
                        >>  306 JUMP_BACKWARD           61 (to 186)
                
-                40     >>  308 JUMP_BACKWARD           71 (to 168)
+                42     >>  308 JUMP_BACKWARD           71 (to 168)
                        >>  310 JUMP_BACKWARD          102 (to 108)
                
-                45     >>  312 LOAD_FAST                1 (fun)
+                47     >>  312 LOAD_FAST                1 (fun)
                            314 LOAD_ATTR                2 (parameters)
                            324 GET_ITER
                        >>  326 FOR_ITER                70 (to 468)
                            328 STORE_FAST               4 (param)
                
-                46         330 LOAD_FAST                1 (fun)
+                48         330 LOAD_FAST                1 (fun)
                            332 LOAD_ATTR                6 (state_variables_written)
                            342 POP_JUMP_FORWARD_IF_FALSE    61 (to 466)
                
-                47         344 LOAD_FAST                1 (fun)
+                49         344 LOAD_FAST                1 (fun)
                            346 LOAD_ATTR                5 (nodes)
                            356 GET_ITER
                        >>  358 FOR_ITER                53 (to 466)
                            360 STORE_FAST               5 (n)
                
-                48         362 LOAD_GLOBAL             15 (NULL + str)
+                50         362 LOAD_GLOBAL             15 (NULL + str)
                            374 LOAD_FAST                4 (param)
                            376 PRECALL                  1
                            380 CALL                     1
                            390 LOAD_GLOBAL             15 (NULL + str)
                            402 LOAD_FAST                5 (n)
                            404 PRECALL                  1
                            408 CALL                     1
                            418 CONTAINS_OP              0
                            420 POP_JUMP_FORWARD_IF_FALSE    21 (to 464)
                
-                49         422 LOAD_FAST                2 (used_params)
+                51         422 LOAD_FAST                2 (used_params)
                            424 LOAD_METHOD              8 (add)
                            446 LOAD_FAST                4 (param)
                            448 PRECALL                  1
                            452 CALL                     1
                            462 POP_TOP
                        >>  464 JUMP_BACKWARD           54 (to 358)
                        >>  466 JUMP_BACKWARD           71 (to 326)
                
-                50     >>  468 LOAD_FAST                1 (fun)
+                52     >>  468 LOAD_FAST                1 (fun)
                            470 LOAD_ATTR                2 (parameters)
                            480 GET_ITER
-                       >>  482 FOR_ITER               121 (to 726)
+                       >>  482 FOR_ITER               153 (to 790)
                            484 STORE_FAST               4 (param)
                
-                51         486 LOAD_FAST                1 (fun)
+                53         486 LOAD_FAST                1 (fun)
                            488 LOAD_ATTR                9 (external_calls_as_expressions)
                            498 GET_ITER
-                       >>  500 FOR_ITER               111 (to 724)
+                       >>  500 FOR_ITER               143 (to 788)
                            502 STORE_FAST               6 (external)
                
-                52         504 LOAD_GLOBAL              1 (NULL + isinstance)
+                54         504 LOAD_GLOBAL              1 (NULL + isinstance)
                            516 LOAD_FAST                6 (external)
                            518 LOAD_ATTR               10 (_called)
                            528 LOAD_GLOBAL             22 (na)
                            540 LOAD_ATTR               12 (NewArray)
                            550 PRECALL                  2
                            554 CALL                     2
                            564 POP_JUMP_FORWARD_IF_FALSE     1 (to 568)
                
-                53         566 JUMP_BACKWARD           34 (to 500)
+                55         566 JUMP_BACKWARD           34 (to 500)
                
-                54     >>  568 BUILD_LIST               0
-                           570 LOAD_FAST                6 (external)
-                           572 LOAD_ATTR               13 (arguments)
-                           582 LIST_EXTEND              1
-                           584 LOAD_FAST                6 (external)
-                           586 LOAD_ATTR               10 (_called)
-                           596 LOAD_ATTR               14 (_expression)
-                           606 LIST_APPEND              1
-                           608 GET_ITER
-                       >>  610 FOR_ITER                55 (to 722)
-                           612 STORE_FAST               7 (arg)
-               
-                55         614 LOAD_GLOBAL             15 (NULL + str)
-                           626 LOAD_FAST                7 (arg)
-                           628 PRECALL                  1
-                           632 CALL                     1
-                           642 LOAD_GLOBAL             15 (NULL + str)
-                           654 LOAD_FAST                4 (param)
-                           656 PRECALL                  1
-                           660 CALL                     1
-                           670 COMPARE_OP               2 (==)
-                           676 POP_JUMP_FORWARD_IF_FALSE    21 (to 720)
-               
-                56         678 LOAD_FAST                2 (used_params)
-                           680 LOAD_METHOD              8 (add)
-                           702 LOAD_FAST                4 (param)
-                           704 PRECALL                  1
-                           708 CALL                     1
-                           718 POP_TOP
-                       >>  720 JUMP_BACKWARD           56 (to 610)
-               
-                54     >>  722 JUMP_BACKWARD          112 (to 500)
-               
-                51     >>  724 JUMP_BACKWARD          122 (to 482)
-               
-                57     >>  726 LOAD_GLOBAL             31 (NULL + len)
-                           738 LOAD_GLOBAL              7 (NULL + set)
-                           750 LOAD_FAST                1 (fun)
-                           752 LOAD_ATTR                2 (parameters)
-                           762 PRECALL                  1
-                           766 CALL                     1
-                           776 LOAD_FAST                2 (used_params)
-                           778 BINARY_OP                1 (&)
-                           782 PRECALL                  1
-                           786 CALL                     1
-                           796 STORE_FAST               8 (intersection_len)
-               
-                58         798 LOAD_FAST                8 (intersection_len)
-                           800 LOAD_GLOBAL             31 (NULL + len)
-                           812 LOAD_FAST                1 (fun)
-                           814 LOAD_ATTR                2 (parameters)
-                           824 PRECALL                  1
-                           828 CALL                     1
-                           838 COMPARE_OP               3 (!=)
-                           844 RETURN_VALUE
+                56     >>  568 LOAD_GLOBAL              1 (NULL + isinstance)
+                           580 LOAD_FAST                6 (external)
+                           582 LOAD_ATTR               10 (_called)
+                           592 LOAD_GLOBAL             26 (nc)
+                           604 LOAD_ATTR               14 (NewContract)
+                           614 PRECALL                  2
+                           618 CALL                     2
+                           628 POP_JUMP_FORWARD_IF_FALSE     1 (to 632)
+               
+                57         630 JUMP_BACKWARD           66 (to 500)
+               
+                58     >>  632 BUILD_LIST               0
+                           634 LOAD_FAST                6 (external)
+                           636 LOAD_ATTR               15 (arguments)
+                           646 LIST_EXTEND              1
+                           648 LOAD_FAST                6 (external)
+                           650 LOAD_ATTR               10 (_called)
+                           660 LOAD_ATTR               16 (_expression)
+                           670 LIST_APPEND              1
+                           672 GET_ITER
+                       >>  674 FOR_ITER                55 (to 786)
+                           676 STORE_FAST               7 (arg)
+               
+                59         678 LOAD_GLOBAL             15 (NULL + str)
+                           690 LOAD_FAST                7 (arg)
+                           692 PRECALL                  1
+                           696 CALL                     1
+                           706 LOAD_GLOBAL             15 (NULL + str)
+                           718 LOAD_FAST                4 (param)
+                           720 PRECALL                  1
+                           724 CALL                     1
+                           734 COMPARE_OP               2 (==)
+                           740 POP_JUMP_FORWARD_IF_FALSE    21 (to 784)
+               
+                60         742 LOAD_FAST                2 (used_params)
+                           744 LOAD_METHOD              8 (add)
+                           766 LOAD_FAST                4 (param)
+                           768 PRECALL                  1
+                           772 CALL                     1
+                           782 POP_TOP
+                       >>  784 JUMP_BACKWARD           56 (to 674)
+               
+                58     >>  786 JUMP_BACKWARD          144 (to 500)
+               
+                53     >>  788 JUMP_BACKWARD          154 (to 482)
+               
+                61     >>  790 LOAD_FAST                1 (fun)
+                           792 LOAD_ATTR               17 (name)
+                           802 LOAD_CONST               3 ('constructor')
+                           804 COMPARE_OP               2 (==)
+                           810 POP_JUMP_FORWARD_IF_FALSE    89 (to 990)
+               
+                62         812 LOAD_FAST                1 (fun)
+                           814 LOAD_ATTR               18 (explicit_base_constructor_calls)
+                           824 GET_ITER
+                       >>  826 FOR_ITER                81 (to 990)
+                           828 STORE_FAST               8 (base_call)
+               
+                63         830 LOAD_FAST                0 (self)
+                           832 LOAD_METHOD             19 (_is_strange_constructor)
+                           854 LOAD_FAST                8 (base_call)
+                           856 PRECALL                  1
+                           860 CALL                     1
+                           870 POP_JUMP_FORWARD_IF_TRUE    58 (to 988)
+               
+                64         872 LOAD_FAST                1 (fun)
+                           874 LOAD_ATTR                2 (parameters)
+                           884 GET_ITER
+                       >>  886 FOR_ITER                50 (to 988)
+                           888 STORE_FAST               9 (param_cur)
+               
+                65         890 LOAD_FAST                8 (base_call)
+                           892 LOAD_ATTR                2 (parameters)
+                           902 GET_ITER
+                       >>  904 FOR_ITER                40 (to 986)
+                           906 STORE_FAST              10 (param_base)
+               
+                66         908 LOAD_GLOBAL             41 (NULL + is_dependent)
+                           920 LOAD_FAST               10 (param_base)
+                           922 LOAD_FAST                9 (param_cur)
+                           924 LOAD_FAST                8 (base_call)
+                           926 PRECALL                  3
+                           930 CALL                     3
+                           940 POP_JUMP_FORWARD_IF_FALSE    21 (to 984)
+               
+                67         942 LOAD_FAST                2 (used_params)
+                           944 LOAD_METHOD              8 (add)
+                           966 LOAD_FAST                9 (param_cur)
+                           968 PRECALL                  1
+                           972 CALL                     1
+                           982 POP_TOP
+                       >>  984 JUMP_BACKWARD           41 (to 904)
+               
+                65     >>  986 JUMP_BACKWARD           51 (to 886)
+                       >>  988 JUMP_BACKWARD           82 (to 826)
+               
+                68     >>  990 LOAD_GLOBAL             43 (NULL + len)
+                          1002 LOAD_GLOBAL              7 (NULL + set)
+                          1014 LOAD_FAST                1 (fun)
+                          1016 LOAD_ATTR                2 (parameters)
+                          1026 PRECALL                  1
+                          1030 CALL                     1
+                          1040 LOAD_FAST                2 (used_params)
+                          1042 BINARY_OP                1 (&)
+                          1046 PRECALL                  1
+                          1050 CALL                     1
+                          1060 STORE_FAST              11 (intersection_len)
+               
+                69        1062 LOAD_FAST               11 (intersection_len)
+                          1064 LOAD_GLOBAL             43 (NULL + len)
+                          1076 LOAD_FAST                1 (fun)
+                          1078 LOAD_ATTR                2 (parameters)
+                          1088 PRECALL                  1
+                          1092 CALL                     1
+                          1102 COMPARE_OP               3 (!=)
+                          1108 RETURN_VALUE
                consts
                   'Checks if setter sets smth to a storage variable and if function parameters are used when setting'
                   True
                   False
-               names      ('isinstance', 'Function', 'parameters', 'set', 'internal_calls', 'nodes', 'state_variables_written', 'str', 'add', 'external_calls_as_expressions', '_called', 'na', 'NewArray', 'arguments', '_expression', 'len')
-               varnames   ('self', 'fun', 'used_params', 'fin', 'param', 'n', 'external', 'arg', 'intersection_len')
+                  'constructor'
+               names      ('isinstance', 'Function', 'parameters', 'set', 'internal_calls', 'nodes', 'state_variables_written', 'str', 'add', 'external_calls_as_expressions', '_called', 'na', 'NewArray', 'nc', 'NewContract', 'arguments', '_expression', 'name', 'explicit_base_constructor_calls', '_is_strange_constructor', 'is_dependent', 'len')
+               varnames   ('self', 'fun', 'used_params', 'fin', 'param', 'n', 'external', 'arg', 'base_call', 'param_cur', 'param_base', 'intersection_len')
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py'
                name       '_is_strange_setter'
-               firstlineno 26
+               firstlineno 28
                lnotab
                   0x02022a0104020e0204011c030cfe040102022a0112011201360102ff12
-                  032cfc040512010e0112013c012e01120112013e0102012e0140012cfe02
-                  fd02064801
+                  032cfc040512010e0112013c012e01120112013e0102013e0102012e0140
+                  012cfe02fb0208160112012a011201120122012cfe04034801
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000005300
-                60           0 RESUME                   0
+                71           0 RESUME                   0
                
-                62           2 LOAD_FAST                0 (self)
+                73           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_is_strange_setter)
                             26 LOAD_FAST                1 (fun)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 RETURN_VALUE
                consts
                   'Checks if constructor sets nothing'
                names      ('_is_strange_setter',)
                varnames   ('self', 'fun')
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py'
                name       '_is_strange_constructor'
-               firstlineno 60
+               firstlineno 71
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 11
                flags     : 3
                code
@@ -451,134 +544,134 @@
                   000000000000007c046a0b0000000000000000a6010000ab010000000000
                   00000064046b030000000072157c00a00c00000000000000000000000000
                   000000000000007c04a6010000ab0100000000000000007d057c05722d7c
                   01a00500000000000000000000000000000000000000007c00a00d000000
                   0000000000000000000000000000000000640564067c04640764086705a6
                   010000ab010000000000000000a6010000ab01000000000000000001008c
                   cf8ce27c015300
-                64           0 RESUME                   0
+                75           0 RESUME                   0
                
-                66           2 BUILD_LIST               0
+                77           2 BUILD_LIST               0
                              4 STORE_FAST               1 (res)
                
-                67           6 LOAD_FAST                0 (self)
+                78           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (compilation_unit)
                             18 LOAD_ATTR                1 (contracts_derived)
                             28 GET_ITER
                        >>   30 FOR_ITER               225 (to 482)
                             32 STORE_FAST               2 (contract)
                
-                68          34 LOAD_FAST                2 (contract)
+                79          34 LOAD_FAST                2 (contract)
                             36 LOAD_ATTR                2 (is_interface)
                             46 POP_JUMP_FORWARD_IF_TRUE   216 (to 480)
                
-                69          48 BUILD_LIST               0
+                80          48 BUILD_LIST               0
                             50 STORE_FAST               3 (overriden_funtions)
                
-                70          52 LOAD_FAST                2 (contract)
+                81          52 LOAD_FAST                2 (contract)
                             54 LOAD_ATTR                3 (functions)
                             64 GET_ITER
                        >>   66 FOR_ITER               206 (to 480)
                             68 STORE_FAST               4 (f)
                
-                71          70 LOAD_FAST                4 (f)
+                82          70 LOAD_FAST                4 (f)
                             72 LOAD_ATTR                4 (parameters)
                             82 POP_JUMP_FORWARD_IF_FALSE   197 (to 478)
                
-                72          84 LOAD_CONST               1 (False)
+                83          84 LOAD_CONST               1 (False)
                             86 STORE_FAST               5 (x)
                
-                73          88 LOAD_FAST                3 (overriden_funtions)
+                84          88 LOAD_FAST                3 (overriden_funtions)
                             90 LOAD_METHOD              5 (append)
                
-                74         112 LOAD_FAST                2 (contract)
+                85         112 LOAD_FAST                2 (contract)
                            114 LOAD_METHOD              6 (get_functions_overridden_by)
                            136 LOAD_FAST                4 (f)
                            138 PRECALL                  1
                            142 CALL                     1
                
-                73         152 PRECALL                  1
+                84         152 PRECALL                  1
                            156 CALL                     1
                            166 POP_TOP
                
-                76         168 LOAD_FAST                4 (f)
+                87         168 LOAD_FAST                4 (f)
                            170 LOAD_ATTR                7 (name)
                            180 LOAD_CONST               2 ('constructor')
                            182 COMPARE_OP               2 (==)
                            188 POP_JUMP_FORWARD_IF_FALSE    22 (to 234)
                
-                77         190 LOAD_FAST                0 (self)
+                88         190 LOAD_FAST                0 (self)
                            192 LOAD_METHOD              8 (_is_strange_constructor)
                            214 LOAD_FAST                4 (f)
                            216 PRECALL                  1
                            220 CALL                     1
                            230 STORE_FAST               5 (x)
                            232 JUMP_FORWARD            75 (to 384)
                
-                79     >>  234 LOAD_FAST                4 (f)
+                90     >>  234 LOAD_FAST                4 (f)
                            236 LOAD_ATTR                7 (name)
                            246 LOAD_METHOD              9 (startswith)
                            268 LOAD_CONST               3 ('set')
                            270 PRECALL                  1
                            274 CALL                     1
                
-                78         284 POP_JUMP_FORWARD_IF_FALSE    49 (to 384)
+                89         284 POP_JUMP_FORWARD_IF_FALSE    49 (to 384)
                
-                80         286 LOAD_FAST                4 (f)
+                91         286 LOAD_FAST                4 (f)
                            288 LOAD_FAST                3 (overriden_funtions)
                            290 CONTAINS_OP              1
                            292 POP_JUMP_FORWARD_IF_FALSE    45 (to 384)
                
-                81         294 LOAD_GLOBAL             21 (NULL + len)
+                92         294 LOAD_GLOBAL             21 (NULL + len)
                            306 LOAD_FAST                4 (f)
                            308 LOAD_ATTR               11 (nodes)
                            318 PRECALL                  1
                            322 CALL                     1
                            332 LOAD_CONST               4 (0)
                            334 COMPARE_OP               3 (!=)
                            340 POP_JUMP_FORWARD_IF_FALSE    21 (to 384)
                
-                83         342 LOAD_FAST                0 (self)
+                94         342 LOAD_FAST                0 (self)
                            344 LOAD_METHOD             12 (_is_strange_setter)
                            366 LOAD_FAST                4 (f)
                            368 PRECALL                  1
                            372 CALL                     1
                            382 STORE_FAST               5 (x)
                
-                84     >>  384 LOAD_FAST                5 (x)
+                95     >>  384 LOAD_FAST                5 (x)
                            386 POP_JUMP_FORWARD_IF_FALSE    45 (to 478)
                
-                85         388 LOAD_FAST                1 (res)
+                96         388 LOAD_FAST                1 (res)
                            390 LOAD_METHOD              5 (append)
                
-                86         412 LOAD_FAST                0 (self)
+                97         412 LOAD_FAST                0 (self)
                            414 LOAD_METHOD             13 (generate_result)
                
-                88         436 LOAD_CONST               5 ('Function')
+                99         436 LOAD_CONST               5 ('Function')
                
-                89         438 LOAD_CONST               6 (' ')
+               100         438 LOAD_CONST               6 (' ')
                
-                90         440 LOAD_FAST                4 (f)
+               101         440 LOAD_FAST                4 (f)
                
-                91         442 LOAD_CONST               7 (' is a strange setter. ')
+               102         442 LOAD_CONST               7 (' is a strange setter. ')
                
-                92         444 LOAD_CONST               8 ('Nothing is set in constructor or set in a function without using function parameters\n')
+               103         444 LOAD_CONST               8 ('Nothing is set in constructor or set in a function without using function parameters\n')
                
-                87         446 BUILD_LIST               5
+                98         446 BUILD_LIST               5
                
-                86         448 PRECALL                  1
+                97         448 PRECALL                  1
                            452 CALL                     1
                
-                85         462 PRECALL                  1
+                96         462 PRECALL                  1
                            466 CALL                     1
                            476 POP_TOP
                        >>  478 JUMP_BACKWARD          207 (to 66)
                        >>  480 JUMP_BACKWARD          226 (to 30)
                
-                97     >>  482 LOAD_FAST                1 (res)
+               108     >>  482 LOAD_FAST                1 (res)
                            484 RETURN_VALUE
                consts
                   'Main function'
                   False
                   'constructor'
                   'set'
                   0
@@ -588,29 +681,29 @@
                   'Nothing is set in constructor or set in a function without using function parameters\n'
                names      ('compilation_unit', 'contracts_derived', 'is_interface', 'functions', 'parameters', 'append', 'get_functions_overridden_by', 'name', '_is_strange_constructor', 'startswith', 'len', 'nodes', '_is_strange_setter', 'generate_result')
                varnames   ('self', 'res', 'contract', 'overriden_funtions', 'f', 'x')
                freevars   ()
                cellvars   ()
                filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py'
                name       '_detect'
-               firstlineno 64
+               firstlineno 75
                lnotab
                   0x020204011c010e01040112010e010401180128ff100316012c0232ff02
                   02080130022a01040118011802020102010201020102fb02ff0eff140c
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'ARGUMENT', 'HELP', 'DetectorClassification', 'HIGH', 'IMPACT', 'MEDIUM', 'CONFIDENCE', 'WIKI', 'WIKI_TITLE', 'WIKI_DESCRIPTION', 'WIKI_EXPLOIT_SCENARIO', 'WIKI_RECOMMENDATION', 'Function', 'bool', '_is_strange_setter', '_is_strange_constructor', 'List', 'Output', '_detect')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py'
          name       'StrangeSetter'
-         firstlineno 8
-         lnotab 0x0a010404040104010e010e0302ff0203040104010401040210221004
+         firstlineno 10
+         lnotab 0x0a010404040104010e010e0302ff02030401040104010402102b1004
       'StrangeSetter'
-   names      ('typing', 'List', 'slither.utils.output', 'Output', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.core.expressions.new_array', 'core', 'expressions', 'new_array', 'na', 'StrangeSetter')
+   names      ('typing', 'List', 'slither.utils.output', 'Output', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.core.expressions.new_array', 'core', 'expressions', 'new_array', 'na', 'slither.core.expressions.new_contract', 'new_contract', 'nc', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'StrangeSetter')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/strange_setter.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0110010c011803
+   lnotab 0x00ff02010c010c0110010c01180118010c03
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/timelock_controller.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/timelock_controller.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2817
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/token_fallback.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/token_fallback.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 1645
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/tx_gasprice_warning.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/tx_gasprice_warning.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 1855
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/uni_v2.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/uni_v2.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 22658
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/unprotected_initialize.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/unprotected_initialize.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3212
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/__pycache__/unprotected_setter.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/__pycache__/unprotected_setter.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 2842
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/aave/__pycache__/flashloan_callback.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/aave/__pycache__/flashloan_callback.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 3990
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/aave/flashloan_callback.py` & `slitherin-0.7.0/slitherin/detectors/aave/flashloan_callback.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrary_call/__pycache__/arbitrary_call.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/arbitrary_call/__pycache__/arbitrary_call.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5af17165 (Thu Dec  7 16:22:50 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 9136
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrary_call/arbitrary_call.py` & `slitherin-0.7.0/slitherin/detectors/arbitrary_call/arbitrary_call.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/arbitrum_prevrandao_difficulty.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/arbitrum_prevrandao_difficulty.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
-files sz: 3128
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 3135
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
       045a040100640064046c056d065a060100640064056c076d085a086d095a
       090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d0100640064
       086c0e6d0f5a0f0100640064096c106d115a1101006400640a6c126d135a
-      136d145a140100640b640c6c156d165a16010002004700640d8400640e65
+      136d145a1401006400640b6c156d165a16010002004700640c8400640d65
       08a6030000ab0300000000000000005a1764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
@@ -83,26 +83,26 @@
                114 IMPORT_NAME             18 (slither.core.declarations.solidity_variables)
                116 IMPORT_FROM             19 (SolidityVariableComposed)
                118 STORE_NAME              19 (SolidityVariableComposed)
                120 IMPORT_FROM             20 (SolidityFunction)
                122 STORE_NAME              20 (SolidityFunction)
                124 POP_TOP
    
-    15         126 LOAD_CONST              11 (3)
-               128 LOAD_CONST              12 (('ARBITRUM_KEY',))
-               130 IMPORT_NAME             21 (consts)
+    15         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST              11 (('ARBITRUM_KEY',))
+               130 IMPORT_NAME             21 (slitherin.consts)
                132 IMPORT_FROM             22 (ARBITRUM_KEY)
                134 STORE_NAME              22 (ARBITRUM_KEY)
                136 POP_TOP
    
     18         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              13 (<code object ArbitrumPrevrandaoDifficulty, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py", line 18>)
+               142 LOAD_CONST              12 (<code object ArbitrumPrevrandaoDifficulty, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py", line 18>)
                144 MAKE_FUNCTION            0
-               146 LOAD_CONST              14 ('ArbitrumPrevrandaoDifficulty')
+               146 LOAD_CONST              13 ('ArbitrumPrevrandaoDifficulty')
                148 LOAD_NAME                8 (AbstractDetector)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME              23 (ArbitrumPrevrandaoDifficulty)
                166 LOAD_CONST               1 (None)
                168 RETURN_VALUE
    consts
@@ -113,15 +113,14 @@
       ('Node',)
       ('AbstractDetector', 'DetectorClassification')
       ('Function',)
       ('EventCall',)
       ('is_dependent',)
       ('SolidityCall',)
       ('SolidityVariableComposed', 'SolidityFunction')
-      3
       ('ARBITRUM_KEY',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
@@ -498,15 +497,15 @@
          freevars   ()
          cellvars   ()
          filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py'
          name       'ArbitrumPrevrandaoDifficulty'
          firstlineno 18
          lnotab 0x0a010404040202ff02030e010e02040104010401040202ff02041c14
       'ArbitrumPrevrandaoDifficulty'
-   names      ('os', 'typing', 'List', 'slither.utils.output', 'Output', 'slither.core.cfg.node', 'Node', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.slithir.operations.event_call', 'EventCall', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'slither.slithir.operations', 'SolidityCall', 'slither.core.declarations.solidity_variables', 'SolidityVariableComposed', 'SolidityFunction', 'consts', 'ARBITRUM_KEY', 'ArbitrumPrevrandaoDifficulty')
+   names      ('os', 'typing', 'List', 'slither.utils.output', 'Output', 'slither.core.cfg.node', 'Node', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.slithir.operations.event_call', 'EventCall', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'slither.slithir.operations', 'SolidityCall', 'slither.core.declarations.solidity_variables', 'SolidityVariableComposed', 'SolidityFunction', 'slitherin.consts', 'ARBITRUM_KEY', 'ArbitrumPrevrandaoDifficulty')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c010c010c0110010c010c010c010c0110050c03
```

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/block_number_timestamp.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/block_number_timestamp.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xcce3cd65 (Thu Feb 15 10:13:32 2024 UTC)
-files sz: 3328
+moddate:  0x9efd3966 (Tue May  7 10:08:30 2024 UTC)
+files sz: 3335
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
       045a040100640064046c056d065a060100640064056c076d085a086d095a
       090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d0100640064
       086c0e6d0f5a0f0100640064096c106d115a1101006400640a6c126d135a
-      136d145a140100640b640c6c156d165a16010002004700640d8400640e65
+      136d145a1401006400640b6c156d165a16010002004700640c8400640d65
       08a6030000ab0300000000000000005a1764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
@@ -83,26 +83,26 @@
                114 IMPORT_NAME             18 (slither.core.declarations.solidity_variables)
                116 IMPORT_FROM             19 (SolidityVariableComposed)
                118 STORE_NAME              19 (SolidityVariableComposed)
                120 IMPORT_FROM             20 (SolidityFunction)
                122 STORE_NAME              20 (SolidityFunction)
                124 POP_TOP
    
-    15         126 LOAD_CONST              11 (3)
-               128 LOAD_CONST              12 (('ARBITRUM_KEY',))
-               130 IMPORT_NAME             21 (consts)
+    15         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST              11 (('ARBITRUM_KEY',))
+               130 IMPORT_NAME             21 (slitherin.consts)
                132 IMPORT_FROM             22 (ARBITRUM_KEY)
                134 STORE_NAME              22 (ARBITRUM_KEY)
                136 POP_TOP
    
     18         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              13 (<code object ArbitrumBlockNumberTimestamp, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/block_number_timestamp.py", line 18>)
+               142 LOAD_CONST              12 (<code object ArbitrumBlockNumberTimestamp, file "/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/block_number_timestamp.py", line 18>)
                144 MAKE_FUNCTION            0
-               146 LOAD_CONST              14 ('ArbitrumBlockNumberTimestamp')
+               146 LOAD_CONST              13 ('ArbitrumBlockNumberTimestamp')
                148 LOAD_NAME                8 (AbstractDetector)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME              23 (ArbitrumBlockNumberTimestamp)
                166 LOAD_CONST               1 (None)
                168 RETURN_VALUE
    consts
@@ -113,15 +113,14 @@
       ('Node',)
       ('AbstractDetector', 'DetectorClassification')
       ('Function',)
       ('EventCall',)
       ('is_dependent',)
       ('SolidityCall',)
       ('SolidityVariableComposed', 'SolidityFunction')
-      3
       ('ARBITRUM_KEY',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
@@ -497,15 +496,15 @@
          freevars   ()
          cellvars   ()
          filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/block_number_timestamp.py'
          name       'ArbitrumBlockNumberTimestamp'
          firstlineno 18
          lnotab 0x0a010404040104010e010e02040202ff02030401040104021c14
       'ArbitrumBlockNumberTimestamp'
-   names      ('os', 'typing', 'List', 'slither.utils.output', 'Output', 'slither.core.cfg.node', 'Node', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.slithir.operations.event_call', 'EventCall', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'slither.slithir.operations', 'SolidityCall', 'slither.core.declarations.solidity_variables', 'SolidityVariableComposed', 'SolidityFunction', 'consts', 'ARBITRUM_KEY', 'ArbitrumBlockNumberTimestamp')
+   names      ('os', 'typing', 'List', 'slither.utils.output', 'Output', 'slither.core.cfg.node', 'Node', 'slither.detectors.abstract_detector', 'AbstractDetector', 'DetectorClassification', 'slither.core.declarations', 'Function', 'slither.slithir.operations.event_call', 'EventCall', 'slither.analyses.data_dependency.data_dependency', 'is_dependent', 'slither.slithir.operations', 'SolidityCall', 'slither.core.declarations.solidity_variables', 'SolidityVariableComposed', 'SolidityFunction', 'slitherin.consts', 'ARBITRUM_KEY', 'ArbitrumBlockNumberTimestamp')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/ndkirillov/Applications/slitherin/slitherin/detectors/arbitrum/block_number_timestamp.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c010c010c0110010c010c010c010c0110050c03
```

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrum/__pycache__/solidity_version.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/arbitrum/__pycache__/solidity_version.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py` & `slitherin-0.7.0/slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from slither.analyses.data_dependency.data_dependency import is_dependent
 from slither.slithir.operations import SolidityCall
 from slither.core.declarations.solidity_variables import (
     SolidityVariableComposed,
     SolidityFunction,
 )
 
-from ...consts import ARBITRUM_KEY
+from slitherin.consts import ARBITRUM_KEY
 
 
 class ArbitrumPrevrandaoDifficulty(AbstractDetector):
     """
     Sees if `prevRandao` or `difficulty` is used inside an Arbitrum contract (as they return constant `1` in Arbitrum)
     """
```

### Comparing `slitherin-0.6.1/slitherin/detectors/arbitrum/block_number_timestamp.py` & `slitherin-0.7.0/slitherin/detectors/arbitrum/block_number_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from slither.analyses.data_dependency.data_dependency import is_dependent
 from slither.slithir.operations import SolidityCall
 from slither.core.declarations.solidity_variables import (
     SolidityVariableComposed,
     SolidityFunction,
 )
 
-from ...consts import ARBITRUM_KEY
+from slitherin.consts import ARBITRUM_KEY
 
 
 class ArbitrumBlockNumberTimestamp(AbstractDetector):
     """
     Sees if `block.number` or `block.timtestamp` is used inside an Arbitrum contract
     """
```

### Comparing `slitherin-0.6.1/slitherin/detectors/before_token_transfer.py` & `slitherin-0.7.0/slitherin/detectors/before_token_transfer.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/call_forward_to_protected.py` & `slitherin-0.7.0/slitherin/detectors/call_forward_to_protected.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/double_entry_token_possibility.py` & `slitherin-0.7.0/slitherin/detectors/double_entry_token_possibility.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/dubious_typecast.py` & `slitherin-0.7.0/slitherin/detectors/dubious_typecast.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/ecrecover.py` & `slitherin-0.7.0/slitherin/detectors/ecrecover.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/event_setter.py` & `slitherin-0.7.0/slitherin/detectors/event_setter.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/falsy_only_eoa_modifier.py` & `slitherin-0.7.0/slitherin/detectors/falsy_only_eoa_modifier.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/for_continue_increment.py` & `slitherin-0.7.0/slitherin/detectors/for_continue_increment.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/inconsistent_nonreentrant.py` & `slitherin-0.7.0/slitherin/detectors/inconsistent_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/magic_number.py` & `slitherin-0.7.0/slitherin/detectors/magic_number.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/multiple_storage_read.py` & `slitherin-0.7.0/slitherin/detectors/multiple_storage_read.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/nft_approve_warning.py` & `slitherin-0.7.0/slitherin/detectors/nft_approve_warning.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from slither.detectors.abstract_detector import AbstractDetector, DetectorClassification
 from typing import List
 from slither.core.cfg.node import Node
 from slither.core.declarations import Function, SolidityVariableComposed
+from slither.core.declarations.function_contract import FunctionContract
 from slither.analyses.data_dependency.data_dependency import is_dependent
 
-
+SAFE_ERC20_LIB_SIG = "safeTransferFrom(address,address,address,uint256)"
 class NftApproveWarning(AbstractDetector):
     """
     Sees if contract contains erc721.[safe]TransferFrom(from, ...) where from parameter is not related to msg.sender
     """
 
     ARGUMENT = 'pess-nft-approve-warning' # slither will launch the detector with slither.py --detect nft-approve-warning
     HELP = '[safe]TransferFrom(from,...) - from parameter is not related to msg.sender'
     IMPACT = DetectorClassification.MEDIUM
     CONFIDENCE = DetectorClassification.LOW
 
     WIKI = 'https://ventral.digital/posts/2022/8/18/sznsdaos-bountyboard-unauthorized-transferfrom-vulnerability'
-    WIKI_TITLE = 'NFT Approve Warning'
+    WIKI_TITLE = 'Token Approve Warning'
     WIKI_DESCRIPTION = "In [safe]TransferFrom() from parameter must be related to msg.sender"
     WIKI_EXPLOIT_SCENARIO = '-'
     WIKI_RECOMMENDATION = 'from parameter must be related to msg.sender'
 
-    _signatures=["transferFrom(address,address,uint256)", "safeTransferFrom(address,address,uint256,bytes)", "safeTransferFrom(address,address,uint256)"]
+    _signatures=["transferFrom(address,address,uint256)", "safeTransferFrom(address,address,uint256,bytes)", "safeTransferFrom(address,address,uint256)", 
+                 SAFE_ERC20_LIB_SIG, # SafeERC20.safeTransferFrom
+                 "safeTransferFrom(address,address,uint256,uint256,bytes)", "safeBatchTransferFrom(address,address,uint256[],uint256[],bytes)"] # ERC1155 
 
     def _detect_arbitrary_from(self, f: Function):
         all_high_level_calls = [
             f_called[1].solidity_signature
             for f_called in f.high_level_calls
             if isinstance(f_called[1], Function)
         ]
@@ -44,15 +47,16 @@
         for node in nodes:
             for ir in node.irs:
                 if (
                     hasattr(ir, 'function')
                     and hasattr(ir.function, 'solidity_signature')
                     and ir.function.solidity_signature in self._signatures
                 ):
-                    is_from_sender = is_dependent(ir.arguments[0], SolidityVariableComposed("msg.sender"), node.function.contract)
+                    is_from_sender = ir.function.solidity_signature !=  SAFE_ERC20_LIB_SIG and is_dependent(ir.arguments[0], SolidityVariableComposed("msg.sender"), node.function.contract) or \
+                                    ir.function.solidity_signature ==  SAFE_ERC20_LIB_SIG and is_dependent(ir.arguments[1], SolidityVariableComposed("msg.sender"), node.function.contract)
                     # is_from_self = is_dependent(ir.arguments[0], SolidityVariable("this"), node.function.contract)
                     if (not is_from_sender): # and not is_from_self
                         irList.append(ir.node)
         return irList
 
 
     def _detect(self):
```

### Comparing `slitherin-0.6.1/slitherin/detectors/potential_arith_overflow.py` & `slitherin-0.7.0/slitherin/detectors/potential_arith_overflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     errors = []
                     for x in irs[:-1]:
                         (response_res, response_errors, _) = self._has_op_overflowing_sub_expression(x, expected_bits)
                         has_problems |= response_res
                         errors.extend(response_errors)
                     if has_problems:
                         final_results.append((node, str(irs[-1].lvalue._type), errors))
-                if len(irs) > 0 and isinstance(irs[-1], ops.Return) and len(fun.return_type) == 1 and str(fun.return_type[0]) in INT_TYPES: # @todo currently works only with single returns
+                if len(irs) > 0 and isinstance(irs[-1], ops.Return) and fun.return_type is not None and len(fun.return_type) == 1 and str(fun.return_type[0]) in INT_TYPES: # @todo currently works only with single returns
                     expected_bits_cut = str(fun.return_type[0]).removeprefix("uint").removeprefix("int")
                     expected_bits = int(256 if not expected_bits_cut else expected_bits_cut)
                     has_problems = False
                     errors = []
                     for x in irs[:-1]:
                         (response_res, response_errors, _) = self._has_op_overflowing_sub_expression(x, expected_bits)
                         has_problems |= response_res
@@ -111,8 +111,8 @@
                 if vulnerable_expressions:
                     info = [f, f" contains integer variables whose type is larger than the type of one of its intermediate expressions. Consider casting sub expressions explicitly as they might lead to unexpected overflow:\n"]
                     for (node, node_final_type, op_with_ret_type) in vulnerable_expressions:
                         info += ["\tIn `", node, "` intermidiate expressions returns type of lower order:", "\n"]
                         for (op, op_ret_type) in op_with_ret_type:
                             info += ["\t\t`", str(op), f"` returns {op_ret_type}, but the type of the resulting expression is {node_final_type}.", "\n"]
                     res.append(self.generate_result(info))
-        return res
+        return res
```

### Comparing `slitherin-0.6.1/slitherin/detectors/public_vs_external.py` & `slitherin-0.7.0/slitherin/detectors/public_vs_external.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/read_only_reentrancy.py` & `slitherin-0.7.0/slitherin/detectors/read_only_reentrancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 from collections import namedtuple, defaultdict
 from typing import Dict, List, Set
 from slither.core.variables.variable import Variable
 from slither.core.declarations import Function
 from slither.core.cfg.node import NodeType, Node, Contract
 from slither.detectors.abstract_detector import DetectorClassification
-from .reentrancy.reentrancy import (
+from slitherin.detectors.reentrancy.reentrancy import (
     Reentrancy,
     to_hashable,
     AbstractState,
     union_dict,
     _filter_if,
     is_subset,
 )
```

### Comparing `slitherin-0.6.1/slitherin/detectors/reentrancy/__pycache__/reentrancy.cpython-311.pyc` & `slitherin-0.7.0/slitherin/detectors/reentrancy/__pycache__/reentrancy.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4a737065 (Wed Dec  6 13:12:42 2023 UTC)
+moddate:  0x9942fd65 (Fri Mar 22 08:34:33 2024 UTC)
 files sz: 10769
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `slitherin-0.6.1/slitherin/detectors/reentrancy/reentrancy.py` & `slitherin-0.7.0/slitherin/detectors/reentrancy/reentrancy.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/strange_setter.py` & `slitherin-0.7.0/slitherin/detectors/strange_setter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List
 from slither.utils.output import Output
 from slither.detectors.abstract_detector import AbstractDetector, DetectorClassification
 from slither.core.declarations import Function
 import slither.core.expressions.new_array as na
+import slither.core.expressions.new_contract as nc
+from slither.analyses.data_dependency.data_dependency import is_dependent
 
 
 class StrangeSetter(AbstractDetector):
     """
     Sees if contract contains a setter, that does not change contract storage variables or that does not use arguments for an external call.
     """
 
@@ -47,17 +49,26 @@
                 for n in fun.nodes:
                     if str(param) in str(n):
                         used_params.add(param)
         for param in fun.parameters:
             for external in fun.external_calls_as_expressions:
                 if isinstance(external._called, na.NewArray):
                     continue
+                if isinstance(external._called, nc.NewContract): # skip new contract calls, idk how to get arguments passed to creation
+                    continue
                 for arg in [*external.arguments, external._called._expression]:
                     if str(arg) == str(param):
                         used_params.add(param)
+        if fun.name == "constructor":
+            for base_call in fun.explicit_base_constructor_calls:
+                if not self._is_strange_constructor(base_call):
+                    for param_cur in fun.parameters:
+                        for param_base in base_call.parameters:
+                            if is_dependent(param_base, param_cur, base_call):
+                                used_params.add(param_cur)
         intersection_len = len(set(fun.parameters) & used_params)
         return intersection_len != len(fun.parameters)
 
     def _is_strange_constructor(self, fun: Function) -> bool:
         """Checks if constructor sets nothing"""
         return self._is_strange_setter(fun)
```

### Comparing `slitherin-0.6.1/slitherin/detectors/timelock_controller.py` & `slitherin-0.7.0/slitherin/detectors/timelock_controller.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/token_fallback.py` & `slitherin-0.7.0/slitherin/detectors/token_fallback.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/tx_gasprice_warning.py` & `slitherin-0.7.0/slitherin/detectors/tx_gasprice_warning.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/uni_v2.py` & `slitherin-0.7.0/slitherin/detectors/uni_v2.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/unprotected_initialize.py` & `slitherin-0.7.0/slitherin/detectors/unprotected_initialize.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/detectors/unprotected_setter.py` & `slitherin-0.7.0/slitherin/detectors/unprotected_setter.py`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/utils/deflat_tokens.json` & `slitherin-0.7.0/slitherin/utils/deflat_tokens.json`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin/utils/rebase_tokens.json` & `slitherin-0.7.0/slitherin/utils/rebase_tokens.json`

 * *Files identical despite different names*

### Comparing `slitherin-0.6.1/slitherin.egg-info/PKG-INFO` & `slitherin-0.7.0/slitherin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: slitherin
-Version: 0.6.1
+Version: 0.7.0
 Summary: Pessimistic security Slither detectors
 Home-page: https://github.com/pessimistic-io/slitherin
 Author: Pessimistic.io
 Author-email: info@pessimistic.io
 License: AGPL-3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: slither-analyzer>=0.10.0
 
-#  Slitherin by Pessimistic.io
+# Slitherin by Pessimistic.io
 
 [![Blog](https://img.shields.io/badge/Blog-Link-blue?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://blog.pessimistic.io/)
 [![Our Website](https://img.shields.io/badge/By-pessimistic.io-green?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://pessimistic.io/)
 [![Mail](https://img.shields.io/badge/Mail-gm%40pessimistic.io-orange?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](mailto:gm@pessimistic.io)
 
 **Welcome!** We are the [pessimistic.io](https://pessimistic.io/) team, and in recent months we have been actively developing our [own **Slither detectors**](https://github.com/pessimistic-io/slitherin/tree/develop/slitherin/detectors) to help with code review and audit process. This repository contains everything you may require to work with them!
 
@@ -112,14 +112,15 @@
 | [Call Forward To Protected](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/call_forward_to_protected.py)                  | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/call_forward_to_protected.md)             | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/call_forward_to_protected_test.sol)                                                  | 0                                                                                                                |
 | [Before Token Transfer](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/before_token_transfer.py)                          | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/before_token_transfer.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/before_token_transfer_test.sol)                                                      | 2                                                                                                                |
 | [For Continue Increment](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/for_continue_increment.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/for_continue_increment.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/for_continue_increment.sol)                                                         | 0                                                                                                                |
 | [AAVE Flasloan Callback](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/aave/flashloan_callback.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/aave/flashloan_callback.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/AaveFlashloanCallback.sol)                                                         | 0                                                                                                                |
 | [Arbitrary Call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/arbitrary_call.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/arbitrary_call_test.sol)                                                         | 0                                                                                                                |
 | [Elliptic Curve Recover](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/ecrecover.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/ecrecover.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/ecrecover.sol)                                                         | 0                                                                                                                |
 | [Public vs External](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/public_vs_external.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/public_vs_external.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/public_vs_external_test.sol)                                                         | 0                                                                                                                |
+| [Balancer Read-only Reentrancy](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/balancer/balancer_readonly_reentrancy.py)                        | [Explore](https://github.com/pessimistic-io/slitherin/blob/master/docs/balancer/readonly_reentrancy.md)                 | [Test](https://github.com/pessimistic-io/slitherin/blob/master/tests/balancer/readonly_reentrancy_test.sol)                                                         | 0                                                                                                                |
 
 **Please note:**
 
 - *Valid - issues included in reports and fixed by developers (January 2023 - June 2023).
 
 - There are two detectors which have several checks inside: [pess-uni-v2](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/uni_v2.py) and [arbitrary-call](https://github.com/pessimistic-io/slitherin/blob/master/slitherin/detectors/arbitrary_call/arbitrary_call.py).
```

### Comparing `slitherin-0.6.1/slitherin.egg-info/SOURCES.txt` & `slitherin-0.7.0/slitherin.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 slitherin/__init__.py
 slitherin/cli.py
 slitherin/consts.py
+slitherin/napalm.py
 slitherin.egg-info/PKG-INFO
 slitherin.egg-info/SOURCES.txt
 slitherin.egg-info/dependency_links.txt
 slitherin.egg-info/entry_points.txt
 slitherin.egg-info/requires.txt
 slitherin.egg-info/top_level.txt
 slitherin/__pycache__/__init__.cpython-311.pyc
@@ -24,14 +25,15 @@
 slitherin/detectors/falsy_only_eoa_modifier.py
 slitherin/detectors/for_continue_increment.py
 slitherin/detectors/inconsistent_nonreentrant.py
 slitherin/detectors/magic_number.py
 slitherin/detectors/multiple_storage_read.py
 slitherin/detectors/nft_approve_warning.py
 slitherin/detectors/potential_arith_overflow.py
+slitherin/detectors/price_manipulation.py
 slitherin/detectors/public_vs_external.py
 slitherin/detectors/read_only_reentrancy.py
 slitherin/detectors/strange_setter.py
 slitherin/detectors/timelock_controller.py
 slitherin/detectors/token_fallback.py
 slitherin/detectors/tx_gasprice_warning.py
 slitherin/detectors/uni_v2.py
@@ -47,14 +49,15 @@
 slitherin/detectors/__pycache__/falsy_only_eoa_modifier.cpython-311.pyc
 slitherin/detectors/__pycache__/for_continue_increment.cpython-311.pyc
 slitherin/detectors/__pycache__/inconsistent_nonreentrant.cpython-311.pyc
 slitherin/detectors/__pycache__/magic_number.cpython-311.pyc
 slitherin/detectors/__pycache__/multiple_storage_read.cpython-311.pyc
 slitherin/detectors/__pycache__/nft_approve_warning.cpython-311.pyc
 slitherin/detectors/__pycache__/potential_arith_overflow.cpython-311.pyc
+slitherin/detectors/__pycache__/price_manipulation.cpython-311.pyc
 slitherin/detectors/__pycache__/public_vs_external.cpython-311.pyc
 slitherin/detectors/__pycache__/read_only_reentrancy.cpython-311.pyc
 slitherin/detectors/__pycache__/strange_setter.cpython-311.pyc
 slitherin/detectors/__pycache__/timelock_controller.cpython-311.pyc
 slitherin/detectors/__pycache__/token_fallback.cpython-311.pyc
 slitherin/detectors/__pycache__/tx_gasprice_warning.cpython-311.pyc
 slitherin/detectors/__pycache__/uni_v2.cpython-311.pyc
@@ -62,18 +65,26 @@
 slitherin/detectors/__pycache__/unprotected_setter.cpython-311.pyc
 slitherin/detectors/aave/__init__.py
 slitherin/detectors/aave/flashloan_callback.py
 slitherin/detectors/aave/__pycache__/__init__.cpython-311.pyc
 slitherin/detectors/aave/__pycache__/flashloan_callback.cpython-311.pyc
 slitherin/detectors/arbitrary_call/arbitrary_call.py
 slitherin/detectors/arbitrary_call/__pycache__/arbitrary_call.cpython-311.pyc
+slitherin/detectors/arbitrum/arbitrum_chainlink_price_feed.py
 slitherin/detectors/arbitrum/arbitrum_prevrandao_difficulty.py
 slitherin/detectors/arbitrum/block_number_timestamp.py
+slitherin/detectors/arbitrum/__pycache__/arbitrum_chainlink_price_feed.cpython-311.pyc
 slitherin/detectors/arbitrum/__pycache__/arbitrum_prevrandao_difficulty.cpython-311.pyc
 slitherin/detectors/arbitrum/__pycache__/block_number_timestamp.cpython-311.pyc
 slitherin/detectors/arbitrum/__pycache__/solidity_version.cpython-311.pyc
+slitherin/detectors/balancer/balancer_readonly_reentrancy.py
+slitherin/detectors/balancer/__pycache__/balancer_readonly_reentrancy.cpython-311.pyc
+slitherin/detectors/curve/curve_readonly_reentrancy.py
+slitherin/detectors/curve/__pycache__/curve_readonly_reentrancy.cpython-311.pyc
 slitherin/detectors/reentrancy/__init__.py
 slitherin/detectors/reentrancy/reentrancy.py
 slitherin/detectors/reentrancy/__pycache__/__init__.cpython-311.pyc
 slitherin/detectors/reentrancy/__pycache__/reentrancy.cpython-311.pyc
+slitherin/detectors/vyper/reentrancy_curve_vyper_version.py
+slitherin/detectors/vyper/__pycache__/reentrancy_curve_vyper_version.cpython-311.pyc
 slitherin/utils/deflat_tokens.json
 slitherin/utils/rebase_tokens.json
```

