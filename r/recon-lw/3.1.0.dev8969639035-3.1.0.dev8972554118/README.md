# Comparing `tmp/recon_lw-3.1.0.dev8969639035.tar.gz` & `tmp/recon_lw-3.1.0.dev8972554118.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recon_lw-3.1.0.dev8969639035.tar", last modified: Mon May  6 13:07:58 2024, max compression
+gzip compressed data, was "recon_lw-3.1.0.dev8972554118.tar", last modified: Mon May  6 16:38:41 2024, max compression
```

## Comparing `recon_lw-3.1.0.dev8969639035.tar` & `recon_lw-3.1.0.dev8972554118.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/example/
--rw-r--r--   0 runner    (1001) docker     (127)    27554 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/example/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 13:07:39.000000 recon_lw-3.1.0.dev8969639035/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/StateStream.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/basic_recon_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/recon_event_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/message_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/one_many.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/pair_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/ts_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/event_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/recon_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/adapter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/equal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/empty_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/any_val.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/refdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/amend_reject.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/filter_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/non_empty_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/session_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/
--rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/one_many.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/pair_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/recon_lw_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/fields_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/exec_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/field_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/match_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/category_displayer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/category_table_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matcher_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/missing_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-06 13:07:58.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.728243 recon_lw-3.1.0.dev8972554118/example/
+-rw-r--r--   0 runner    (1001) docker     (127)    27554 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/example/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 16:38:25.000000 recon_lw-3.1.0.dev8972554118/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.728243 recon_lw-3.1.0.dev8972554118/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/StateStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/basic_recon_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/recon_event_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/processor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/processor/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/message_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/one_many.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/pair_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/ts_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/type/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/type/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/event_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/recon_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.732243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/adapter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.736243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/equal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.736243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/condition/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/condition/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.736243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/empty_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.736243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/any_val.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/refdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/amend_reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/filter_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/non_empty_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/session_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_handling_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_handling_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.740243 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_name_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_name_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/context/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/simple_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/simple_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/one_many.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/pair_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/recon_lw_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.744243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/viewer/fields_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/exec_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/issue_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/error_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/field_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/match_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/category_displayer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.748243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/style_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/style_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/style_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/style_provider/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/types/category_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/viewer/missing_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_metadata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/recon_lw/reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.728243 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 16:38:41.000000 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-06 16:38:41.000000 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:38:41.000000 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 16:38:41.000000 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 16:38:41.000000 recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:38:41.752243 recon_lw-3.1.0.dev8972554118/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-06 16:37:56.000000 recon_lw-3.1.0.dev8972554118/test/test_recon_ob.py
```

### Comparing `recon_lw-3.1.0.dev8969639035/PKG-INFO` & `recon_lw-3.1.0.dev8972554118/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recon_lw
-Version: 3.1.0.dev8969639035
+Version: 3.1.0.dev8972554118
 Summary: recon_lw
 Home-page: https://github.com/th2-net/recon-lw
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Recon-lw
```

### Comparing `recon_lw-3.1.0.dev8969639035/README.md` & `recon_lw-3.1.0.dev8972554118/README.md`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/example/example.ipynb` & `recon_lw-3.1.0.dev8972554118/example/example.ipynb`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/EventsSaver.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/SequenceCache.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/StateStream.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/StateStream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/basic_recon_event.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/basic_recon_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             diffs = []
         self.diffs: List[ReconEventDiff] = diffs
         self.matching_key = matching_key
 
     @property
     def body(self):
         full_body = {
-            **self.body,
+            **self._body,
             "diff": list(map(lambda d: d.to_dict(), self.diffs)),
             "key": self.matching_key,
         }
         return full_body
 
     @body.setter
     def body(self, body):
```

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/event_type.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/event_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,21 @@
     MISS_LEFT='MissLeft',
     MISS_RIGHT='MissRight',
 )
 
 
 class ReconEventType(Enum):
     # TODO
+    #   1)
     #   I don't sure that we need `BasicRecon` prefix
     #   What's the sense to use it? We used it on the *** project because
     #   we had recon with name Basic.
     #   Actually a user can have any names for Events
+    #   2)
+    #   Probably it's better to change to Just class (no Enum)
     BasicReconRoot = 'BasicReconRoot'
     BasicReconMatch = 'BasicReconMatch'
     BasicReconMissLeft = 'BasicReconMissLeft'
     BasicReconMissRight = 'BasicReconMissRight'
 
 
     # The comment as reminder
```

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/recon_event_diff.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/basic_recon_event/recon_event_diff.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/cache/processor/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/message_utils.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/message_utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/one_many.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/one_many.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/pair_one.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/rule/pair_one.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/stream.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/ts_converters.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/ts_converters.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/recon_utils.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/core/utility/recon_utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/adapter_context.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/adapter_context.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/compound.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/compound.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/simple.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/adapter/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/adapter.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/adapter.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/check_result.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/check_result.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/equal.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/check_rule/equal.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/function.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/condition/function.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/__init__.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/boolean.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/boolean.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/chain.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/condition.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/condition.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/datetime.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/datetime.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dictionary.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/dictionary.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/list.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/list.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/mapping.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/mapping.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/type.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/converter/type.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/simple.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_checker/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/__init__.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/any_val.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/any_val.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/cache.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/cache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/concat.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/concat.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/condition.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/condition.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/constant.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/constant.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/converter.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/converter.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/dictionary.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/dictionary.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/list.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/list.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/one_of.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/one_of.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/refdata.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/field_extractor/refdata.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/amend_reject.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/amend_reject.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/field.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/field.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/filter_chain.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/filter_chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/non_empty_field.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/filter/non_empty_field.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/simple.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/interpretation_functions/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/recon_ob_stats.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/interpretation/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/LastStateMatcher.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/LiveObjectsCache.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/StateSequenceGenerator.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/TimeCacheMatcher.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/collect_matcher/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/flush_function/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/simple.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/context/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/init_function/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_copy.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/simple_copy.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_original.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/key_functions/simple_original.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/separator.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/matching_key_extractor/separator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/matching.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/matching.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/utils.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/old/utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob_cross_stream.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_oe_ob.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/one_many.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/one_many.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/pair_one.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/matching/stream_matcher/pair_one.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/recon_lw_entrypoint.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/recon_lw_entrypoint.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/fields_viewer.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/coverage/viewer/fields_viewer.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/known_issues/issue.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/basic.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/basic.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/basic.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/event_category/basic.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/context.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/context.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from collections import defaultdict
 from typing import Dict
 
 import tabulate
 
-from recon_lw.reporting.match_diff.categorizer.event_category.base import EventCategory
+from recon_lw.reporting.match_diff.categorizer.event_category.base import \
+    EventCategory
 
 
 class ErrorCategoriesStats:
-    def __init__(self, error_categories: Dict[EventCategory, int]=None):
+    def __init__(self, error_categories: Dict[EventCategory, int] = None):
         if not error_categories:
             error_categories = defaultdict(lambda: defaultdict(lambda: 0))
         self.error_categories = error_categories
 
     def add_error_category(self, recon_name, error_category: EventCategory):
         self.error_categories[recon_name][error_category] += 1
 
     def _get_sorted_error_categories(self, recon_name):
         return [
             (k, v) for k, v in sorted(
-                self.error_categories[recon_name].items(), key=lambda x: x[1], reverse=True
+                self.error_categories[recon_name].items(), key=lambda x: x[1],
+                reverse=True
             )
         ]
 
     def get_table_stats(self, recon_name: str):
         return tabulate.tabulate(
             self._get_sorted_error_categories(recon_name),
             headers=['category', 'count'],
             tablefmt='html'
         )
-
-
```

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_examples.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/error_examples.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/field_problems.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/categorizer/types/field_problems.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/category_displayer.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/category_displayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,17 +215,16 @@
                 That should be a function that
                     - takes: a message (usually real exchange message in dict
                         format).
                     - returns: a list of matching-keys
                         e.g. ['key-field1-val:key-field2-val']
             message_content_provider:
                 Function or `IExampleContentProvider` class that provides
-                FIXME:
-                    ЭТО НУЖНО ДЛЯ ТОГО, ЧТОБЫ ОРДЕР ХИСТОРИ СТРОИТЬ.
-                    НЕ ДУМАЮ, ЧТО ЭТО ДОЛЖНО В ТАКОМ ВИДЕ ЗДЕСЬ ОСТАТЬСЯ!!
+                CategoryTableView
+
             recon_context:
             error_example_displayer:
         """
         self.context: ReconErrorStatsContext = recon_stats_context
         self.events: Data[dict] = recon_context.get_recon_events()
         self.messages: Data = messages
         self.mfr = recon_context.get_mfr()
@@ -247,14 +246,18 @@
                 to Recon result events.
         """
         if self._cache is not None:
             return self._cache
 
         self._cache = {}
 
+        # FIXME:
+        #   The problem here that we use self.mfr.get_id(message)
+        #   But we can actually provide events. (any stream, not only messages)
+
         for message in self.messages:
             msg_id = self.mfr.get_id(message)
             if self.context.error_examples.is_id_affected(msg_id):
                 self._cache[msg_id] = message
         return self._cache
 
     def display_report(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/color_provider/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/base.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/default.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/style_provider/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/category_table_view.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/types/category_table_view.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/utils.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/match_diff/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/utils.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/missing_message.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/missing_messages/viewer/missing_message.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/context.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/recon_context/context.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/stats.py` & `recon_lw-3.1.0.dev8972554118/recon_lw/reporting/stats/stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/PKG-INFO` & `recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recon-lw
-Version: 3.1.0.dev8969639035
+Version: 3.1.0.dev8972554118
 Summary: recon_lw
 Home-page: https://github.com/th2-net/recon-lw
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Recon-lw
```

### Comparing `recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/SOURCES.txt` & `recon_lw-3.1.0.dev8972554118/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/setup.py` & `recon_lw-3.1.0.dev8972554118/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.1.0.dev8969639035/test/test_recon_ob.py` & `recon_lw-3.1.0.dev8972554118/test/test_recon_ob.py`

 * *Files identical despite different names*
