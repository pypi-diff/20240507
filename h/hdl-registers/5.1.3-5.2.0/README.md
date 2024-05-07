# Comparing `tmp/hdl_registers-5.1.3.tar.gz` & `tmp/hdl_registers-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdl_registers-5.1.3.tar", last modified: Wed Apr  3 07:05:23 2024, max compression
+gzip compressed data, was "hdl_registers-5.2.0.tar", last modified: Tue May  7 11:54:35 2024, max compression
```

## Comparing `hdl_registers-5.1.3.tar` & `hdl_registers-5.2.0.tar`

### file list

```diff
@@ -1,141 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.262746 hdl_registers-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-03 07:05:23.262746 hdl_registers-5.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.238746 hdl_registers-5.1.3/hdl_registers/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/about.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.242746 hdl_registers-5.1.3/hdl_registers/constant/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/bit_vector_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/boolean_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/float_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/integer_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/string_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.242746 hdl_registers-5.1.3/hdl_registers/constant/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/test_bit_vector_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/test_boolean_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/test_float_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/test_integer_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/constant/test/test_string_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.242746 hdl_registers-5.1.3/hdl_registers/field/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/bit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/bit_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/register_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/register_field_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.246746 hdl_registers-5.1.3/hdl_registers/field/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_bit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_bit_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_register_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/field/test/test_register_field_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.246746 hdl_registers-5.1.3/hdl_registers/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.246746 hdl_registers-5.1.3/hdl_registers/generator/c/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/c/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/c/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.246746 hdl_registers-5.1.3/hdl_registers/generator/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/cpp_generator_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/cpp/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/cpp/test/test_register_cpp_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/html/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/constant_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/html_generator_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/html_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/register_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/html/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/test/test_html_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/html/test/test_register_html_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/python/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/python/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/python/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/python/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/python/test/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    19018 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/register_code_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/register_code_generator_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.250746 hdl_registers-5.1.3/hdl_registers/generator/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generator_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/test/test_reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.254746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.254746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.254746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/test/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/record_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/register_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.254746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/check_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    23560 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/read_write_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.254746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_check_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_read_write_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_wait_until_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/vhdl_simulation_generator_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/wait_until_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.258746 hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_record_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_register_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_register_vhdl_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/generator/vhdl/vhdl_generator_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.258746 hdl_registers-5.1.3/hdl_registers/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    15540 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.258746 hdl_registers-5.1.3/hdl_registers/parser/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    18208 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/test/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/test/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/parser/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/register_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/register_list.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/requirements_develop.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.258746 hdl_registers-5.1.3/hdl_registers/test/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/test/test_register_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/hdl_registers/test/test_register_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:05:23.258746 hdl_registers-5.1.3/hdl_registers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-03 07:05:23.000000 hdl_registers-5.1.3/hdl_registers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-03 07:05:23.000000 hdl_registers-5.1.3/hdl_registers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:05:23.000000 hdl_registers-5.1.3/hdl_registers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 07:05:23.000000 hdl_registers-5.1.3/hdl_registers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 07:05:23.000000 hdl_registers-5.1.3/hdl_registers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:05:23.262746 hdl_registers-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 07:05:13.000000 hdl_registers-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.725045 hdl_registers-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-07 11:54:35.725045 hdl_registers-5.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.701045 hdl_registers-5.2.0/hdl_registers/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.705045 hdl_registers-5.2.0/hdl_registers/constant/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/bit_vector_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/boolean_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/float_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/integer_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/string_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.705045 hdl_registers-5.2.0/hdl_registers/constant/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/test_bit_vector_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/test_boolean_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/test_float_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/test_integer_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/constant/test/test_string_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.705045 hdl_registers-5.2.0/hdl_registers/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/bit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/bit_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/register_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14410 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/register_field_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.709045 hdl_registers-5.2.0/hdl_registers/field/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_bit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_bit_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_register_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/field/test/test_register_field_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.709045 hdl_registers-5.2.0/hdl_registers/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.709045 hdl_registers-5.2.0/hdl_registers/generator/c/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/c/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/c/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.709045 hdl_registers-5.2.0/hdl_registers/generator/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/cpp_generator_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.709045 hdl_registers-5.2.0/hdl_registers/generator/cpp/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/cpp/test/test_register_cpp_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.713045 hdl_registers-5.2.0/hdl_registers/generator/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/constant_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/html_generator_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/html_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/register_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.713045 hdl_registers-5.2.0/hdl_registers/generator/html/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/test/test_html_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/html/test/test_register_html_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.713045 hdl_registers-5.2.0/hdl_registers/generator/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35560 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/register_accessor_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.713045 hdl_registers-5.2.0/hdl_registers/generator/python/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.713045 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/test_accessor_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32756 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/test_accessor_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/accessor/test_accessor_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/python/test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/register_code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/register_code_generator_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generator_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/test/test_reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/test/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/record_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/register_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/check_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23560 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/read_write_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.717045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_check_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_read_write_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_wait_until_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/vhdl_simulation_generator_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/wait_until_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.721045 hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_record_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_register_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_register_vhdl_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/generator/vhdl/vhdl_generator_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.721045 hdl_registers-5.2.0/hdl_registers/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15540 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.721045 hdl_registers-5.2.0/hdl_registers/parser/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18208 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/test/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/test/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/parser/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/register_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/register_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/requirements_develop.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.721045 hdl_registers-5.2.0/hdl_registers/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/test/test_register_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/hdl_registers/test/test_register_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:54:35.721045 hdl_registers-5.2.0/hdl_registers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-07 11:54:35.000000 hdl_registers-5.2.0/hdl_registers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 11:54:35.000000 hdl_registers-5.2.0/hdl_registers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:54:35.000000 hdl_registers-5.2.0/hdl_registers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 11:54:35.000000 hdl_registers-5.2.0/hdl_registers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 11:54:35.000000 hdl_registers-5.2.0/hdl_registers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:54:35.725045 hdl_registers-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-07 11:54:25.000000 hdl_registers-5.2.0/setup.py
```

### Comparing `hdl_registers-5.1.3/PKG-INFO` & `hdl_registers-5.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdl_registers
-Version: 5.1.3
+Version: 5.2.0
 Summary: An open-source HDL register interface code generator fast enough to run in real time
 Author: Lukas Vik
 Author-email: 10241915+LukasVik@users.noreply.github.com
 License: BSD 3-Clause License
 Project-URL: Homepage, https://hdl-registers.com
-Project-URL: Documentation, https://hdl-registers.com/
+Project-URL: Documentation, https://hdl-registers.com
 Project-URL: Changelog, https://hdl-registers.com/rst/about/release_notes.html
 Project-URL: Source, https://github.com/hdl-registers/hdl-registers
 Project-URL: Issues, https://github.com/hdl-registers/hdl-registers/issues
 Keywords: python,c,html,asic,generator,fpga,cplusplus,register,vhdl,eda,rtl,csr,axi,axi-lite,register-interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -23,33 +23,33 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Requires-Dist: black
 Requires-Dist: GitPython
 Requires-Dist: PyYAML
 Requires-Dist: rtoml<0.10.0,>=0.9.0
-Requires-Dist: tsfpga>=12.3.1
+Requires-Dist: termcolor
+Requires-Dist: tsfpga>=12.3.2
 Provides-Extra: develop
-Requires-Dist: black; extra == "develop"
 Requires-Dist: flake8; extra == "develop"
 Requires-Dist: GitPython; extra == "develop"
 Requires-Dist: mypy; extra == "develop"
 Requires-Dist: packaging; extra == "develop"
 Requires-Dist: pybadges; extra == "develop"
 Requires-Dist: pycairo; extra == "develop"
 Requires-Dist: PyGObject; extra == "develop"
 Requires-Dist: pylint; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytest-xdist; extra == "develop"
 Requires-Dist: PyYAML; extra == "develop"
-Requires-Dist: rtoml; extra == "develop"
 Requires-Dist: setuptools; extra == "develop"
 Requires-Dist: sphinx; extra == "develop"
 Requires-Dist: sphinx_sitemap; extra == "develop"
 Requires-Dist: sphinx-rtd-theme; extra == "develop"
 Requires-Dist: sphinx-toolbox; extra == "develop"
 Requires-Dist: sphinxcontrib-wavedrom; extra == "develop"
 Requires-Dist: sphinxext-opengraph; extra == "develop"
@@ -121,26 +121,30 @@
 a `TOML/JSON/YAML data file <https://hdl-registers.com/rst/user_guide/toml_format.html>`_
 or the `Python API <https://hdl-registers.com/rst/user_guide/user_guide_python_api.html>`_.
 The following code can be generated:
 
 * `VHDL <https://hdl-registers.com/rst/generator/generator_vhdl.html>`_
 
   * AXI-Lite register file wrapper using records and native VHDL types for values.
-  * Support packages for compact and efficient simulation.
+  * Simulation support packages for compact read/write/wait/checking of register and field values.
 
 * `C++ <https://hdl-registers.com/rst/generator/generator_cpp.html>`_
 
   * Complete class with setters and getters for registers and fields.
   * Includes an abstract interface header for unit test mocking.
 
 * `C header <https://hdl-registers.com/rst/generator/generator_c.html>`_
   with register addresses and field information.
+
 * `HTML <https://hdl-registers.com/rst/generator/generator_html.html>`_
   website with documentation of registers and fields.
 
+* `Python <https://hdl-registers.com/rst/generator/generator_python.html>`_
+  class with methods to read/write/print each register and field on a target device.
+
 The tool can also be extended by
 `writing your own code generator <https://hdl-registers.com/rst/extensions/extensions_custom_generator.html>`_
 using a simple but powerful API.
 
 This project is mature and used in many production environments.
 The maintainers place high focus on quality, with everything having good unit test coverage and a
 thought-out structure.
```

### Comparing `hdl_registers-5.1.3/hdl_registers/__init__.py` & `hdl_registers-5.2.0/hdl_registers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 HDL_REGISTERS_PATH = REPO_ROOT / "hdl_registers"
 HDL_REGISTERS_DOC = REPO_ROOT / "doc"
 HDL_REGISTERS_GENERATED = REPO_ROOT / "generated"
 HDL_REGISTERS_TESTS = REPO_ROOT / "tests"
 HDL_REGISTERS_TOOLS = REPO_ROOT / "tools"
 
-__version__ = "5.1.3"
+__version__ = "5.2.0"
 __doc__ = get_short_slogan()  # pylint: disable=redefined-builtin
```

### Comparing `hdl_registers-5.1.3/hdl_registers/conftest.py` & `hdl_registers-5.2.0/hdl_registers/conftest.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/bit_vector_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/bit_vector_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/boolean_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/boolean_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/float_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/float_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/integer_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/integer_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/string_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/string_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/test/test_bit_vector_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/test/test_bit_vector_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/test/test_boolean_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/test/test_boolean_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/test/test_float_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/test/test_float_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/test/test_integer_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/test/test_integer_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/constant/test/test_string_constant.py` & `hdl_registers-5.2.0/hdl_registers/constant/test/test_string_constant.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/field/bit.py` & `hdl_registers-5.2.0/hdl_registers/field/bit.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         self._base_index = index
         self.description = description
 
         self._default_value = ""
         # Assign self._default_value via setter
         self.default_value = default_value
 
-    @property
-    def base_index(self) -> int:
-        return self._base_index
-
     @property  # type: ignore[override]
     def default_value(self) -> str:
         """
         Getter for private member.
         """
         return self._default_value
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/bit_vector.py` & `hdl_registers-5.2.0/hdl_registers/field/bit_vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 #
 # This file is part of the hdl-registers project, an HDL register generator fast enough to run
 # in real time.
 # https://hdl-registers.com
 # https://github.com/hdl-registers/hdl-registers
 # --------------------------------------------------------------------------------------------------
 
+# Standard libraries
+from typing import Union
+
 # Local folder libraries
 from .register_field import DEFAULT_FIELD_TYPE, RegisterField
 from .register_field_type import FieldType, Fixed
 
 
 class BitVector(RegisterField):
     """
@@ -50,21 +53,36 @@
         self._default_value = ""
         # Assign self._default_value via setter
         self.default_value = default_value
 
         self._field_type = field_type
 
     @property
-    def field_type(self) -> FieldType:
-        return self._field_type
-
-    @property
     def width(self) -> int:
+        """
+        Getter for private member.
+        """
         return self._width
 
+    @property
+    def min_value(self) -> Union[int, float]:
+        """
+        Minimum numeric value this field can assume.
+        Getter for private member.
+        """
+        return self._field_type.min_value(bit_width=self._width)
+
+    @property
+    def max_value(self) -> Union[int, float]:
+        """
+        Maximum numeric value this field can assume.
+        Getter for private member.
+        """
+        return self._field_type.max_value(bit_width=self._width)
+
     def _check_width(self, width: int, field_type: FieldType) -> None:
         """
         Sanity checks for the provided width
         Will raise exception if something is wrong.
         """
         if not isinstance(width, int):
             message = (
@@ -81,18 +99,14 @@
         if isinstance(field_type, Fixed):
             if width != field_type.expected_bit_width:
                 raise ValueError(
                     f'Inconsistent width for bit vector "{self.name}". '
                     f'Field is "{width}" bits, type is "{field_type.expected_bit_width}".'
                 )
 
-    @property
-    def base_index(self) -> int:
-        return self._base_index
-
     @property  # type: ignore[override]
     def default_value(self) -> str:
         """
         Getter for private member.
         """
         return self._default_value
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/enumeration.py` & `hdl_registers-5.2.0/hdl_registers/field/enumeration.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,14 @@
     def width(self) -> int:
         num_elements = len(self._elements)
         num_bits = (num_elements - 1).bit_length() if num_elements > 1 else 1
 
         return num_bits
 
     @property
-    def base_index(self) -> int:
-        return self._base_index
-
-    @property
     def elements(self) -> list[EnumerationElement]:
         """
         Getter for elements.
         """
         return self._elements
 
     def get_element_by_name(self, name: str) -> EnumerationElement:
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/integer.py` & `hdl_registers-5.2.0/hdl_registers/field/integer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # in real time.
 # https://hdl-registers.com
 # https://github.com/hdl-registers/hdl-registers
 # --------------------------------------------------------------------------------------------------
 
 # Local folder libraries
 from .register_field import RegisterField
-from .register_field_type import FieldType, Signed, Unsigned
+from .register_field_type import Signed, Unsigned
 
 
 class Integer(RegisterField):  # pylint: disable=too-many-instance-attributes
     """
     Used to represent an integer field in a register.
     """
 
@@ -47,29 +47,15 @@
         self._max_value = max_value
 
         self._default_value = 0
         # Assign self._default_value via setter
         self.default_value = default_value
 
         # Determines how bits are to be interpreted in 'set_value' and 'get_value'.
-        self._field_type = Signed() if self.is_signed else Unsigned()
-
-    @property
-    def field_type(self) -> FieldType:
-        """
-        Getter for private member.
-        """
-        return self._field_type
-
-    @property
-    def is_signed(self) -> bool:
-        """
-        Returns True if the field can hold negative numbers.
-        """
-        return self._min_value < 0
+        self._field_type = Signed() if min_value < 0 else Unsigned()
 
     @property
     def width(self) -> int:
         # Calculate the width based on the supplied numerical limits.
         error_message = (
             f"Supplied integer range [{self._min_value}, {self._max_value}] does not fit "
             "in a register."
@@ -90,18 +76,14 @@
             max_range = 2 ** (num_bits - 1) - 1
 
             if self._min_value >= min_range and self._max_value <= max_range:
                 return num_bits
 
         raise ValueError(error_message)
 
-    @property
-    def base_index(self) -> int:
-        return self._base_index
-
     def _check_range(self, min_value: int, max_value: int) -> None:
         """
         Perform some sanity checks on user-supplied values.
         Will raise exception if something is wrong,.
         """
         if not isinstance(min_value, int):
             message = (
@@ -123,21 +105,23 @@
                 f"Got: [{min_value}, {max_value}]."
             )
             raise ValueError(message)
 
     @property
     def min_value(self) -> int:
         """
+        Minimum numeric value this field can assume.
         Getter for private member.
         """
         return self._min_value
 
     @property
     def max_value(self) -> int:
         """
+        Maximum numeric value this field can assume.
         Getter for private member.
         """
         return self._max_value
 
     @property  # type: ignore[override]
     def default_value(self) -> int:
         """
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/register_field.py` & `hdl_registers-5.2.0/hdl_registers/field/register_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,30 @@
 
 class RegisterField(ABC):
     """
     Meta class for all register fields (bits, bit vectors, integers, ...).
     Lists a few methods that must be implemented.
     """
 
-    # Must set these two as class members in subclasses.
+    # Must set as class members in subclasses.
     name: str
+    _base_index: int
     description: str
     default_value: Union[str, int]
 
+    # Default type, should be assigned to something else in subclasses when appropriate.
+    _field_type: FieldType = DEFAULT_FIELD_TYPE
+
+    @property
+    def base_index(self) -> int:
+        """
+        The index within the register for the lowest bit of this field.
+        """
+        return self._base_index
+
     @property
     def max_binary_value(self) -> int:
         """
         Get the maximum value, represented as a positive integer, that this
         field can hold given its width.
         """
         result: int = 2**self.width - 1
@@ -50,29 +61,28 @@
 
     @property
     def field_type(self) -> FieldType:
         """
         The field type (Unsigned, Signed, UnsignedFixedPoint, SignedFixedPoint, ...)
         used to interpret the bits of the field.
         """
-        # Default for all RegisterFields
-        return DEFAULT_FIELD_TYPE
+        return self._field_type
 
     @property
-    @abstractmethod
-    def width(self) -> int:
+    def is_signed(self) -> bool:
         """
-        Return the width, in number of bits, that this field occupies.
+        Returns True if the field can hold negative numbers.
         """
+        return self._field_type.is_signed
 
     @property
     @abstractmethod
-    def base_index(self) -> int:
+    def width(self) -> int:
         """
-        The index within the register for the lowest bit of this field.
+        Return the width, in number of bits, that this field occupies.
         """
 
     @property
     @abstractmethod
     def default_value_str(self) -> str:
         """
         Return a formatted string of the default value. The way it shall appear
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/register_field_type.py` & `hdl_registers-5.2.0/hdl_registers/field/register_field_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,114 +8,126 @@
 # --------------------------------------------------------------------------------------------------
 
 # Standard libraries
 from abc import ABC, abstractmethod
 from typing import Optional, Union
 
 
-def _from_unsigned_binary(
-    bit_width: int,
-    unsigned_binary: int,
-    integer_bit_width: Optional[int] = None,
-    fraction_bit_width: int = 0,
+def from_unsigned_binary(
+    num_bits: int,
+    value: int,
+    num_integer_bits: Optional[int] = None,
+    num_fractional_bits: int = 0,
     is_signed: bool = False,
 ) -> Union[int, float]:
     """
-    Convert from an unsigned binary to one of:
-    - unsigned integer
-    - signed integer
-    - unsigned fixed point
-    - signed fixed point
+    Convert from a fixed-point unsigned binary value to one of
 
-    Signed uses two's complement representation.
+    * unsigned integer (Python ``int``)
+    * signed integer (Python ``int``)
+    * unsigned floating-point (Python ``float``)
+    * signed floating-point (Python ``float``)
 
+    Signed types use two's complement representation for the binary value.
     Sources:
-        https://en.wikibooks.org/wiki/Floating_Point/Fixed-Point_Numbers
-        https://vhdlguru.blogspot.com/2010/03/fixed-point-operations-in-vhdl-tutorial.html
+
+    * https://en.wikibooks.org/wiki/Floating_Point/Fixed-Point_Numbers
+    * https://vhdlguru.blogspot.com/2010/03/fixed-point-operations-in-vhdl-tutorial.html
 
     Arguments:
-        bit_width: Width of the field.
-        unsigned_binary: Unsigned binary integer representation of the field.
-        integer_bit_width: If fixed point, the number of bits assigned to the integer part of the
-            field value.
-        fraction_bit_width: If fixed point, the number of bits assigned to the fractional part of
-            the field value.
-        is_signed: Is the field signed (two's complement)?
+        num_bits: Width of the field.
+        value: Unsigned binary integer representation of the value.
+        num_integer_bits: The number of integer bits in the fixed-point ``value``.
+            Might be negative if this is a fixed-point word with only fractional bits.
+        num_fractional_bits: The number of fractional bits in the fixed-point ``value``.
+            Might be negative if this is a fixed-point word with only integer bits.
+        is_signed: If ``True``, the MSB of the ``value`` will be treated as a sign bit.
+            Enables the handling of negative result values.
 
     Return:
-        Native Python representation of the field value.
-        Will be a ``float`` if ``fraction_bit_width`` is non-zero, otherwise it will be an ``int``.
+        Native Python representation of the ``value``.
+        Will be a ``float`` if ``num_fractional_bits`` is non-zero, otherwise it will be an ``int``.
     """
-    integer_bit_width = bit_width if integer_bit_width is None else integer_bit_width
+    num_integer_bits = num_bits if num_integer_bits is None else num_integer_bits
 
-    if integer_bit_width + fraction_bit_width != bit_width:
+    if num_integer_bits + num_fractional_bits != num_bits:
         raise ValueError("Inconsistent bit width")
 
-    value: Union[int, float] = unsigned_binary * 2**-fraction_bit_width
+    result: Union[int, float] = value * 2**-num_fractional_bits
 
     if is_signed:
-        sign_bit = unsigned_binary & (1 << (bit_width - 1))
+        sign_bit = value & (1 << (num_bits - 1))
         if sign_bit != 0:
             # If sign bit is set, compute negative value.
-            value -= 2**integer_bit_width
+            result -= 2**num_integer_bits
 
-    return value
+    return result
 
 
-def _to_unsigned_binary(
-    bit_width: int,
+def to_unsigned_binary(
+    num_bits: int,
     value: Union[int, float],
-    integer_bit_width: Optional[int] = None,
-    fraction_bit_width: int = 0,
+    num_integer_bits: Optional[int] = None,
+    num_fractional_bits: int = 0,
     is_signed: bool = False,
 ) -> int:
     """
-    Convert from one of:
-        - unsigned integer
-        - signed integer
-        - unsigned fixed point
-        - signed fixed point
-    into an unsigned binary.
+    Convert from one of
 
-    Signed uses two's complement representation.
+    * unsigned integer (Python ``int``)
+    * signed integer (Python ``int``)
+    * unsigned floating-point (Python ``float``)
+    * signed floating-point (Python ``float``)
 
+    into an unsigned binary.
+    Signed types use two's complement representation for the binary value.
     Sources:
-        https://en.wikibooks.org/wiki/Floating_Point/Fixed-Point_Numbers
-        https://vhdlguru.blogspot.com/2010/03/fixed-point-operations-in-vhdl-tutorial.html
+
+    * https://en.wikibooks.org/wiki/Floating_Point/Fixed-Point_Numbers
+    * https://vhdlguru.blogspot.com/2010/03/fixed-point-operations-in-vhdl-tutorial.html
 
     Arguments:
-        bit_width: Width of the field.
-        value: Native Python representation of the field value.
-           If ``fraction_bit_width`` is non-zero the value is expected to be a ``float``, otherwise
-           an ``int`` is expected.
-        integer_bit_width: If fixed point, the number of bits assigned to the integer part of the
-            field value.
-        fraction_bit_width: If fixed point, the number of bits assigned to the fractional part of
-            the field value.
-        is_signed: Is the field signed (two's complement)?
+        num_bits: Width of the field.
+        value: Native numeric Python representation of the value.
+            If ``num_fractional_bits`` is non-zero the value is expected to be a ``float``,
+            otherwise an ``int`` is expected.
+        num_integer_bits: The number of integer bits in the target fixed-point word.
+            Might be negative if this is a fixed-point word with only fractional bits.
+        num_fractional_bits: The number of fractional bits in the target fixed-point word.
+            Might be negative if this is a fixed-point word with only integer bits.
+        is_signed: Enables the handling of negative input ``value``.
+            If ``True``, the MSB of the result word will be treated as a sign bit.
 
     Return:
-        Unsigned binary integer representation of the field.
+        Unsigned binary integer representation of the value.
+        Potentially rounded, if the input ``value`` is a floating-point number.
     """
-    integer_bit_width = bit_width if integer_bit_width is None else integer_bit_width
+    num_integer_bits = num_bits if num_integer_bits is None else num_integer_bits
 
-    if integer_bit_width + fraction_bit_width != bit_width:
+    if num_integer_bits + num_fractional_bits != num_bits:
         raise ValueError("Inconsistent bit width")
 
-    binary_value: int = round(value * 2**fraction_bit_width)
+    binary_value: int = round(value * 2**num_fractional_bits)
     if value < 0:
         if is_signed:
-            binary_value += 1 << bit_width
+            binary_value += 1 << num_bits
         else:
             raise ValueError("Attempting to convert negative value to unsigned")
 
     return binary_value
 
 
 class FieldType(ABC):
+    @property
+    @abstractmethod
+    def is_signed(self) -> bool:
+        """
+        Is the field signed (two's complement)?
+        """
+
     @abstractmethod
     def min_value(self, bit_width: int) -> Union[int, float]:
         """
         Minimum representable value for this field type.
 
         Return type is the native Python representation of the value, which depends on the subclass.
         If the subclass has a non-zero number of fractional bits, the value will be a ``float``.
@@ -178,14 +190,16 @@
 
 
 class Unsigned(FieldType):
     """
     Unsigned integer.
     """
 
+    is_signed: bool = False
+
     def min_value(self, bit_width: int) -> int:
         return 0
 
     def max_value(self, bit_width: int) -> int:
         result: int = 2**bit_width - 1
         return result
 
@@ -201,28 +215,30 @@
 
 
 class Signed(FieldType):
     """
     Two's complement signed integer format.
     """
 
+    is_signed: bool = True
+
     def min_value(self, bit_width: int) -> int:
         result: int = -(2 ** (bit_width - 1))
         return result
 
     def max_value(self, bit_width: int) -> int:
         result: int = 2 ** (bit_width - 1) - 1
         return result
 
     def convert_from_unsigned_binary(self, bit_width: int, unsigned_binary: int) -> int:
-        return int(_from_unsigned_binary(bit_width, unsigned_binary, is_signed=True))
+        return int(from_unsigned_binary(num_bits=bit_width, value=unsigned_binary, is_signed=True))
 
     def convert_to_unsigned_binary(self, bit_width: int, value: float) -> int:
         self._check_value_in_range(bit_width, value)
-        return _to_unsigned_binary(bit_width, value, is_signed=True)
+        return to_unsigned_binary(num_bits=bit_width, value=value, is_signed=True)
 
     def __repr__(self) -> str:
         return self.__class__.__name__
 
 
 class Fixed(FieldType, ABC):
     def __init__(self, is_signed: bool, max_bit_index: int, min_bit_index: int):
@@ -236,51 +252,55 @@
         fractional portion.
 
         Arguments:
             is_signed: Is the field signed (two's complement)?
             max_bit_index: Position of the upper bit relative to the decimal point.
             min_bit_index: Position of the lower bit relative to the decimal point.
         """
-        self.is_signed = is_signed
+        self._is_signed = is_signed
         self._integer = Signed() if is_signed else Unsigned()
         self.max_bit_index = max_bit_index
         self.min_bit_index = min_bit_index
         if not self.max_bit_index >= self.min_bit_index:
             raise ValueError("max_bit_index must be >= min_bit_index")
 
         self.integer_bit_width = self.max_bit_index + 1
         self.fraction_bit_width = -self.min_bit_index
         self.expected_bit_width = self.integer_bit_width + self.fraction_bit_width
 
+    @property
+    def is_signed(self) -> bool:
+        return self._is_signed
+
     def min_value(self, bit_width: int) -> float:
         min_integer_value = self._integer.min_value(bit_width)
         min_integer_binary = self._integer.convert_to_unsigned_binary(bit_width, min_integer_value)
         return self.convert_from_unsigned_binary(bit_width, min_integer_binary)
 
     def max_value(self, bit_width: int) -> float:
         max_integer_value = self._integer.max_value(bit_width)
         max_integer_binary = self._integer.convert_to_unsigned_binary(bit_width, max_integer_value)
         return self.convert_from_unsigned_binary(bit_width, max_integer_binary)
 
     def convert_from_unsigned_binary(self, bit_width: int, unsigned_binary: int) -> float:
-        return _from_unsigned_binary(
-            bit_width=bit_width,
-            unsigned_binary=unsigned_binary,
-            integer_bit_width=self.integer_bit_width,
-            fraction_bit_width=self.fraction_bit_width,
+        return from_unsigned_binary(
+            num_bits=bit_width,
+            value=unsigned_binary,
+            num_integer_bits=self.integer_bit_width,
+            num_fractional_bits=self.fraction_bit_width,
             is_signed=self.is_signed,
         )
 
     def convert_to_unsigned_binary(self, bit_width: int, value: float) -> int:
         self._check_value_in_range(bit_width, value)
-        return _to_unsigned_binary(
-            bit_width=bit_width,
+        return to_unsigned_binary(
+            num_bits=bit_width,
             value=value,
-            integer_bit_width=self.integer_bit_width,
-            fraction_bit_width=self.fraction_bit_width,
+            num_integer_bits=self.integer_bit_width,
+            num_fractional_bits=self.fraction_bit_width,
             is_signed=self.is_signed,
         )
 
     def __repr__(self) -> str:
         return f"""{self.__class__.__name__}(\
 max_bit_index={self.max_bit_index},\
 min_bit_index={self.min_bit_index},\
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_bit.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_bit.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_bit_vector.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_bit_vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,50 @@
         width=16,
         default_value="0" * 16,
         field_type=SignedFixedPoint.from_bit_widths(integer_bit_width=8, fraction_bit_width=8),
     )
     assert field.set_value(-0.00390625) == 0b11_11111111_11111100
 
 
+def test_min_and_max_value():
+    bit_vector = BitVector(
+        name="", base_index=0, description="", width=4, default_value="0000", field_type=Unsigned()
+    )
+    assert bit_vector.min_value == 0
+    assert bit_vector.max_value == 15
+
+    bit_vector = BitVector(
+        name="", base_index=0, description="", width=4, default_value="0000", field_type=Signed()
+    )
+    assert bit_vector.min_value == -8
+    assert bit_vector.max_value == 7
+
+    bit_vector = BitVector(
+        name="",
+        base_index=0,
+        description="",
+        width=4,
+        default_value="0000",
+        field_type=UnsignedFixedPoint(1, -2),
+    )
+    assert bit_vector.min_value == 0
+    assert bit_vector.max_value == 3.75
+
+    bit_vector = BitVector(
+        name="",
+        base_index=0,
+        description="",
+        width=4,
+        default_value="0000",
+        field_type=SignedFixedPoint(1, -2),
+    )
+    assert bit_vector.min_value == -2
+    assert bit_vector.max_value == 1.75
+
+
 def test_repr():
     # Check that repr is an actual representation, not just "X object at 0xABCDEF"
     assert "apa" in repr(
         BitVector(name="apa", base_index=0, description="", width=1, default_value="0")
     )
 
     # Different name
```

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_enumeration.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_integer.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_integer.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_register_field.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_register_field.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/field/test/test_register_field_type.py` & `hdl_registers-5.2.0/hdl_registers/field/test/test_register_field_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         (8, -1, 0b11111111),
         (8, 40, 0b00101000),
         (8, -40, 0b11011000),
         (8, 126, 0b01111110),
         (8, -126, 0b10000010),
     ],
 )
-def test_singed(bit_width, value, expected):
+def test_signed(bit_width, value, expected):
     field_type = Signed()
     field_type._check_value_in_range(bit_width, value)
     unsigned = field_type.convert_to_unsigned_binary(bit_width, value)
     assert unsigned == expected
     restored = field_type.convert_from_unsigned_binary(bit_width, unsigned)
     assert restored == value
```

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/c/header.py` & `hdl_registers-5.2.0/hdl_registers/generator/c/header.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/c/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/c/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/cpp_generator_common.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/cpp_generator_common.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/header.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/header.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/implementation.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/implementation.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/interface.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/interface.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/cpp/test/test_register_cpp_generator.py` & `hdl_registers-5.2.0/hdl_registers/generator/cpp/test/test_register_cpp_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/constant_table.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/constant_table.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/html_generator_common.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/html_generator_common.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/html_translator.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/html_translator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/page.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/page.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/register_table.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/register_table.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/test/test_html_translator.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/test/test_html_translator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/html/test/test_register_html_generator.py` & `hdl_registers-5.2.0/hdl_registers/generator/html/test/test_register_html_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/python/pickle.py` & `hdl_registers-5.2.0/hdl_registers/generator/python/pickle.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,41 +76,44 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     # Third party libraries
     from hdl_registers.register_list import RegisterList
 
 THIS_DIR = Path(__file__).parent
+PICKLE_FILE = THIS_DIR / "{self.pickle_file.name}"
 
 
 class {class_name}:
-
     """
-    Instantiate this class to get the RegisterList object for the '{self.name}' module.
+    Instantiate this class to get the ``RegisterList`` object for the
+    ``{self.name}`` register list.
     """
 
     def __new__(cls):
         """
-        Recreate the RegisterList object from binary pickle.
+        Recreate the ``RegisterList`` object from binary pickle.
         """
-        with (THIS_DIR / "{self.pickle_file.name}").open("rb") as file_handle:
+        with PICKLE_FILE.open("rb") as file_handle:
             return pickle.load(file_handle)
 
 
 def get_register_list() -> "RegisterList":
     """
-    Return a RegisterList object with the registers/constants from the '{self.name}' module.
+    Return a ``RegisterList`` object with the registers/constants from the
+    ``{self.name}`` register list.
     Recreated from a Python pickle file.
     """
-    return {class_name}()
+    with PICKLE_FILE.open("rb") as file_handle:
+        return pickle.load(file_handle)
 '''
 
     @property
     def should_create(self) -> bool:
         """
-        Since this generator creates two files, where on is binary, it is impossible to do the
+        Since this generator creates two files, where one is binary, it is impossible to do the
         version/hash check.
         Hence, set it to "always create".
         The mechanism "create if needed" should not be used for this generator anyway, since
         this generator is not designed to run in real-time like e.g. the VHDL generator.
         """
         return True
```

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/python/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/python/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/python/test/test_pickle.py` & `hdl_registers-5.2.0/hdl_registers/generator/python/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/register_code_generator.py` & `hdl_registers-5.2.0/hdl_registers/generator/register_code_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # --------------------------------------------------------------------------------------------------
 
 # Standard libraries
 import datetime
 import re
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any, Optional
 
 # Third party libraries
 from tsfpga.git_utils import get_git_commit, git_commands_are_available
 from tsfpga.svn_utils import get_svn_revision_information, svn_commands_are_available
 from tsfpga.system_utils import create_file, path_relative_to, read_file
 
 # First party libraries
@@ -222,15 +222,15 @@
         ) != self._find_versions_and_hash_of_existing_file(file_path=output_file):
             return True
 
         return False
 
     def _find_versions_and_hash_of_existing_file(
         self, file_path: Path
-    ) -> tuple[Union[None, str], Union[None, str], Union[None, str]]:
+    ) -> tuple[Optional[str], Optional[str], Optional[str]]:
         """
         Returns the matching strings in a tuple. Either field can be ``None`` if nothing found.
         """
         existing_file_content = read_file(file=file_path)
 
         result_package_version = None
         result_generator_version = None
```

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/register_code_generator_helpers.py` & `hdl_registers-5.2.0/hdl_registers/generator/register_code_generator_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def iterate_register_objects(self) -> Iterator[Union[Register, RegisterArray]]:
         """
         Iterate over all register objects in the register list.
         I.e. all plain registers and all register arrays.
         """
         yield from self.register_list.register_objects
 
-    def iterate_registers(self) -> Iterator[tuple[Register, Union[RegisterArray, None]]]:
+    def iterate_registers(self) -> Iterator[tuple[Register, Optional[RegisterArray]]]:
         """
         Iterate over all registers, plain or in array, in the register list.
 
         Return:
             If the register is plain, the array return value in the tuple will be ``None``.
             If the register is in an array, the array return value will conversely be non-``None``.
         """
```

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generation.py` & `hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from hdl_registers.generator.c.header import CHeaderGenerator
 from hdl_registers.generator.cpp.header import CppHeaderGenerator
 from hdl_registers.generator.cpp.implementation import CppImplementationGenerator
 from hdl_registers.generator.cpp.interface import CppInterfaceGenerator
 from hdl_registers.generator.html.constant_table import HtmlConstantTableGenerator
 from hdl_registers.generator.html.page import HtmlPageGenerator
 from hdl_registers.generator.html.register_table import HtmlRegisterTableGenerator
+from hdl_registers.generator.python.accessor import PythonAccessorGenerator
 from hdl_registers.generator.python.pickle import PythonPickleGenerator
 from hdl_registers.generator.vhdl.axi_lite.wrapper import VhdlAxiLiteWrapperGenerator
 from hdl_registers.generator.vhdl.record_package import VhdlRecordPackageGenerator
 from hdl_registers.generator.vhdl.register_package import VhdlRegisterPackageGenerator
 from hdl_registers.generator.vhdl.simulation.read_write_package import (
     VhdlSimulationReadWritePackageGenerator,
 )
@@ -103,7 +104,10 @@
     assert (tmp_path / f"{register_list.name}_regs.html").exists()
 
 
 @pytest.mark.parametrize("register_list", REGISTER_LISTS)
 def test_can_generate_python_without_error(tmp_path, register_list):
     PythonPickleGenerator(register_list, tmp_path).create()
     assert (tmp_path / f"{register_list.name}.py").exists()
+
+    PythonAccessorGenerator(register_list, tmp_path).create()
+    assert (tmp_path / f"{register_list.name}_accessor.py").exists()
```

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generator.py` & `hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/test/test_register_code_generator_helpers.py` & `hdl_registers-5.2.0/hdl_registers/generator/test/test_register_code_generator_helpers.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/test/test_reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/test/test_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/test/test_wrapper.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/test/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/axi_lite/wrapper.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/axi_lite/wrapper.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/record_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/record_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/register_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/register_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/reserved_keywords.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/check_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/check_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/read_write_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/read_write_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_check_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_check_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_read_write_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_read_write_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/test/test_wait_until_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/test/test_wait_until_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/vhdl_simulation_generator_common.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/vhdl_simulation_generator_common.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/simulation/wait_until_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/simulation/wait_until_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_record_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_record_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_register_package.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_register_package.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/test/test_register_vhdl_generator.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/test/test_register_vhdl_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/generator/vhdl/vhdl_generator_common.py` & `hdl_registers-5.2.0/hdl_registers/generator/vhdl/vhdl_generator_common.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/json.py` & `hdl_registers-5.2.0/hdl_registers/parser/json.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/parser.py` & `hdl_registers-5.2.0/hdl_registers/parser/parser.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/test/test_json.py` & `hdl_registers-5.2.0/hdl_registers/parser/test/test_json.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/test/test_parser.py` & `hdl_registers-5.2.0/hdl_registers/parser/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/test/test_toml.py` & `hdl_registers-5.2.0/hdl_registers/parser/test/test_toml.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/test/test_yaml.py` & `hdl_registers-5.2.0/hdl_registers/parser/test/test_yaml.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/toml.py` & `hdl_registers-5.2.0/hdl_registers/parser/toml.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/parser/yaml.py` & `hdl_registers-5.2.0/hdl_registers/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/register.py` & `hdl_registers-5.2.0/hdl_registers/register.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/register_array.py` & `hdl_registers-5.2.0/hdl_registers/register_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
         The index within the register list where array iteration number ``array_index`` starts.
 
         Arguments:
             array_index: The array iteration index.
                 Must be less than the array ``length``.
         """
-        if array_index >= self.length:
+        if not 0 <= array_index < self.length:
             raise ValueError(
                 f'Index {array_index} out of range for register array "{self.name}" '
                 f"of length {self.length}."
             )
 
         return self.base_index + array_index * len(self.registers)
```

### Comparing `hdl_registers-5.1.3/hdl_registers/register_list.py` & `hdl_registers-5.2.0/hdl_registers/register_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,25 +125,35 @@
         register_array = RegisterArray(
             name=name, base_index=base_index, length=length, description=description
         )
 
         self.register_objects.append(register_array)
         return register_array
 
-    def get_register(self, name: str) -> Register:
+    def get_register(self, name: str, register_array_name: Optional[str] = None) -> Register:
         """
         Get a register from this list.
-        Will only find plain registers, not registers in a register array.
         Will raise exception if no register matches.
 
+        If ``register_array_name`` is specified, this method will search for registers within
+        that array.
+        If it is not specified, the method will only search for plain registers (not registers
+        in any arrays).
+
         Arguments:
             name: The name of the register.
+            register_array_name: If the register is within a register array, this is the name of
+                the array.
         Return:
             The register.
         """
+        if register_array_name is not None:
+            register_array = self.get_register_array(name=register_array_name)
+            return register_array.get_register(name=name)
+
         for register_object in self.register_objects:
             if isinstance(register_object, Register) and register_object.name == name:
                 return register_object
 
         raise ValueError(f'Could not find register "{name}" within register list "{self.name}"')
 
     def get_register_array(self, name: str) -> RegisterArray:
@@ -180,23 +190,25 @@
                 index must be specified.
 
         Return:
             The index.
         """
         if register_array_name is None or register_array_index is None:
             # Target is plain register
-            register = self.get_register(register_name)
+            register = self.get_register(name=register_name)
 
             return register.index
 
         # Target is in register array
-        register_array = self.get_register_array(register_array_name)
-        register_array_start_index = register_array.get_start_index(register_array_index)
+        register_array = self.get_register_array(name=register_array_name)
+        register_array_start_index = register_array.get_start_index(
+            array_index=register_array_index
+        )
 
-        register = register_array.get_register(register_name)
+        register = register_array.get_register(name=register_name)
         register_index = register.index
 
         return register_array_start_index + register_index
 
     def add_constant(
         self,
         name: str,
```

### Comparing `hdl_registers-5.1.3/hdl_registers/test/test_register.py` & `hdl_registers-5.2.0/hdl_registers/test/test_register.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-5.1.3/hdl_registers/test/test_register_array.py` & `hdl_registers-5.2.0/hdl_registers/test/test_register_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,7 +111,13 @@
 def test_start_index_with_argument_outside_of_length_should_raise_exception():
     register_array = RegisterArray(name="apa", base_index=0, length=4, description="")
     register_array.append_register(name="hest", mode="r", description="")
 
     with pytest.raises(ValueError) as exception_info:
         register_array.get_start_index(4)
     assert str(exception_info.value) == 'Index 4 out of range for register array "apa" of length 4.'
+
+    with pytest.raises(ValueError) as exception_info:
+        register_array.get_start_index(-1)
+    assert (
+        str(exception_info.value) == 'Index -1 out of range for register array "apa" of length 4.'
+    )
```

### Comparing `hdl_registers-5.1.3/hdl_registers/test/test_register_list.py` & `hdl_registers-5.2.0/hdl_registers/test/test_register_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,36 +116,52 @@
         name="zebra", length=2, description=""
     )
     assert register_array_zebra.base_index == 8
 
 
 def test_get_register():
     register_list = RegisterList(name="apa", source_definition_file=None)
+    apa = register_list.append_register(name="apa", mode="r", description="")
     hest = register_list.append_register(name="hest", mode="r", description="")
-    zebra = register_list.append_register(name="zebra", mode="r", description="")
-    register_list.append_register_array(name="register_array", length=3, description="")
+    register_array = register_list.append_register_array(
+        name="register_array", length=3, description=""
+    )
+    zebra = register_array.append_register(name="zebra", mode="r", description="")
 
-    assert register_list.get_register("hest") is hest
-    assert register_list.get_register("zebra") is zebra
+    assert register_list.get_register(name="apa") is apa
+    assert register_list.get_register(name="hest") is hest
 
     with pytest.raises(ValueError) as exception_info:
-        assert register_list.get_register("non existing") is None
+        assert register_list.get_register(name="non existing") is None
     assert (
         str(exception_info.value)
         == 'Could not find register "non existing" within register list "apa"'
     )
 
     with pytest.raises(ValueError) as exception_info:
-        assert register_list.get_register("register_array") is None
+        register_list.get_register(name="register_array")
     assert (
         str(exception_info.value)
         == 'Could not find register "register_array" within register list "apa"'
     )
     register_list.get_register_array("register_array")
 
+    with pytest.raises(ValueError) as exception_info:
+        register_list.get_register(name="zebra")
+    assert str(exception_info.value) == 'Could not find register "zebra" within register list "apa"'
+
+    assert register_list.get_register(name="zebra", register_array_name="register_array") is zebra
+
+    with pytest.raises(ValueError) as exception_info:
+        register_list.get_register(name="hest", register_array_name="register_array")
+    assert (
+        str(exception_info.value)
+        == 'Could not find register "hest" within register array "register_array"'
+    )
+
 
 def test_get_register_array():
     register_list = RegisterList(name="apa", source_definition_file=None)
     hest = register_list.append_register_array(name="hest", length=3, description="")
     zebra = register_list.append_register_array(name="zebra", length=2, description="")
     register_list.append_register(name="register", mode="r", description="")
```

### Comparing `hdl_registers-5.1.3/hdl_registers.egg-info/PKG-INFO` & `hdl_registers-5.2.0/hdl_registers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdl_registers
-Version: 5.1.3
+Version: 5.2.0
 Summary: An open-source HDL register interface code generator fast enough to run in real time
 Author: Lukas Vik
 Author-email: 10241915+LukasVik@users.noreply.github.com
 License: BSD 3-Clause License
 Project-URL: Homepage, https://hdl-registers.com
-Project-URL: Documentation, https://hdl-registers.com/
+Project-URL: Documentation, https://hdl-registers.com
 Project-URL: Changelog, https://hdl-registers.com/rst/about/release_notes.html
 Project-URL: Source, https://github.com/hdl-registers/hdl-registers
 Project-URL: Issues, https://github.com/hdl-registers/hdl-registers/issues
 Keywords: python,c,html,asic,generator,fpga,cplusplus,register,vhdl,eda,rtl,csr,axi,axi-lite,register-interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -23,33 +23,33 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Requires-Dist: black
 Requires-Dist: GitPython
 Requires-Dist: PyYAML
 Requires-Dist: rtoml<0.10.0,>=0.9.0
-Requires-Dist: tsfpga>=12.3.1
+Requires-Dist: termcolor
+Requires-Dist: tsfpga>=12.3.2
 Provides-Extra: develop
-Requires-Dist: black; extra == "develop"
 Requires-Dist: flake8; extra == "develop"
 Requires-Dist: GitPython; extra == "develop"
 Requires-Dist: mypy; extra == "develop"
 Requires-Dist: packaging; extra == "develop"
 Requires-Dist: pybadges; extra == "develop"
 Requires-Dist: pycairo; extra == "develop"
 Requires-Dist: PyGObject; extra == "develop"
 Requires-Dist: pylint; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: pytest-cov; extra == "develop"
 Requires-Dist: pytest-xdist; extra == "develop"
 Requires-Dist: PyYAML; extra == "develop"
-Requires-Dist: rtoml; extra == "develop"
 Requires-Dist: setuptools; extra == "develop"
 Requires-Dist: sphinx; extra == "develop"
 Requires-Dist: sphinx_sitemap; extra == "develop"
 Requires-Dist: sphinx-rtd-theme; extra == "develop"
 Requires-Dist: sphinx-toolbox; extra == "develop"
 Requires-Dist: sphinxcontrib-wavedrom; extra == "develop"
 Requires-Dist: sphinxext-opengraph; extra == "develop"
@@ -121,26 +121,30 @@
 a `TOML/JSON/YAML data file <https://hdl-registers.com/rst/user_guide/toml_format.html>`_
 or the `Python API <https://hdl-registers.com/rst/user_guide/user_guide_python_api.html>`_.
 The following code can be generated:
 
 * `VHDL <https://hdl-registers.com/rst/generator/generator_vhdl.html>`_
 
   * AXI-Lite register file wrapper using records and native VHDL types for values.
-  * Support packages for compact and efficient simulation.
+  * Simulation support packages for compact read/write/wait/checking of register and field values.
 
 * `C++ <https://hdl-registers.com/rst/generator/generator_cpp.html>`_
 
   * Complete class with setters and getters for registers and fields.
   * Includes an abstract interface header for unit test mocking.
 
 * `C header <https://hdl-registers.com/rst/generator/generator_c.html>`_
   with register addresses and field information.
+
 * `HTML <https://hdl-registers.com/rst/generator/generator_html.html>`_
   website with documentation of registers and fields.
 
+* `Python <https://hdl-registers.com/rst/generator/generator_python.html>`_
+  class with methods to read/write/print each register and field on a target device.
+
 The tool can also be extended by
 `writing your own code generator <https://hdl-registers.com/rst/extensions/extensions_custom_generator.html>`_
 using a simple but powerful API.
 
 This project is mature and used in many production environments.
 The maintainers place high focus on quality, with everything having good unit test coverage and a
 thought-out structure.
```

### Comparing `hdl_registers-5.1.3/hdl_registers.egg-info/SOURCES.txt` & `hdl_registers-5.2.0/hdl_registers.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -63,18 +63,25 @@
 hdl_registers/generator/html/page.py
 hdl_registers/generator/html/register_table.py
 hdl_registers/generator/html/reserved_keywords.py
 hdl_registers/generator/html/test/__init__.py
 hdl_registers/generator/html/test/test_html_translator.py
 hdl_registers/generator/html/test/test_register_html_generator.py
 hdl_registers/generator/python/__init__.py
+hdl_registers/generator/python/accessor.py
 hdl_registers/generator/python/pickle.py
+hdl_registers/generator/python/register_accessor_interface.py
 hdl_registers/generator/python/reserved_keywords.py
 hdl_registers/generator/python/test/__init__.py
 hdl_registers/generator/python/test/test_pickle.py
+hdl_registers/generator/python/test/accessor/__init__.py
+hdl_registers/generator/python/test/accessor/conftest.py
+hdl_registers/generator/python/test/accessor/test_accessor_basic.py
+hdl_registers/generator/python/test/accessor/test_accessor_operations.py
+hdl_registers/generator/python/test/accessor/test_accessor_py.py
 hdl_registers/generator/test/__init__.py
 hdl_registers/generator/test/test_register_code_generation.py
 hdl_registers/generator/test/test_register_code_generator.py
 hdl_registers/generator/test/test_register_code_generator_helpers.py
 hdl_registers/generator/test/test_reserved_keywords.py
 hdl_registers/generator/vhdl/__init__.py
 hdl_registers/generator/vhdl/record_package.py
```

### Comparing `hdl_registers-5.1.3/pyproject.toml` & `hdl_registers-5.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # third party import.
 known_tools_pythonpath = "tools.tools_pythonpath"
 sections = "FUTURE,STDLIB,TOOLS_PYTHONPATH,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
 
 # ------------------------------------------------------------------------------
 [tool.mypy]
-exclude = ['/test_.*\.py$']
+exclude = ['/test_.*\.py$', '/conftest.py$']
 
 # Use strict as a base, and explicitly remove the checks that we do not want.
 strict = true
 
 
 # ------------------------------------------------------------------------------
 [build-system]
```

### Comparing `hdl_registers-5.1.3/setup.py` & `hdl_registers-5.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
 REPO_ROOT = Path(__file__).parent.resolve()
 sys.path.insert(0, str(REPO_ROOT))
 
 # First party libraries
 import hdl_registers
-from hdl_registers.about import get_readme_rst, get_short_slogan
+from hdl_registers.about import REPOSITORY_URL, WEBSITE_URL, get_readme_rst, get_short_slogan
 
 # Duplicated from tsfpga/__init__.py since setup.py may not depend on tsfpga
 DEFAULT_FILE_ENCODING = "utf-8"
 
 REQUIREMENTS_TXT = hdl_registers.HDL_REGISTERS_PATH / "requirements.txt"
 REQUIREMENTS_DEVELOP_TXT = hdl_registers.HDL_REGISTERS_PATH / "requirements_develop.txt"
 PY_TYPED = hdl_registers.HDL_REGISTERS_PATH / "py.typed"
@@ -116,19 +116,19 @@
         #
         install_requires=read_requirements_file(REQUIREMENTS_TXT),
         extras_require=dict(develop=read_requirements_file(REQUIREMENTS_DEVELOP_TXT)),
         #
         python_requires=">=3.9",
         #
         project_urls={
-            "Homepage": "https://hdl-registers.com",
-            "Documentation": "https://hdl-registers.com/",
-            "Changelog": "https://hdl-registers.com/rst/about/release_notes.html",
-            "Source": "https://github.com/hdl-registers/hdl-registers",
-            "Issues": "https://github.com/hdl-registers/hdl-registers/issues",
+            "Homepage": WEBSITE_URL,
+            "Documentation": WEBSITE_URL,
+            "Changelog": f"{WEBSITE_URL}/rst/about/release_notes.html",
+            "Source": REPOSITORY_URL,
+            "Issues": f"{REPOSITORY_URL}/issues",
         },
     )
 
 
 def read_requirements_file(path):
     requirements = []
     with open(path, encoding=DEFAULT_FILE_ENCODING) as file_handle:
```

