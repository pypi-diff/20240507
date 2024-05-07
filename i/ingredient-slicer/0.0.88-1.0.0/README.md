# Comparing `tmp/ingredient_slicer-0.0.88.tar.gz` & `tmp/ingredient_slicer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-0.0.88.tar", last modified: Thu Apr 18 12:58:21 2024, max compression
+gzip compressed data, was "ingredient_slicer-1.0.0.tar", last modified: Tue May  7 12:26:18 2024, max compression
```

## Comparing `ingredient_slicer-0.0.88.tar` & `ingredient_slicer-1.0.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.332093 ingredient_slicer-0.0.88/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.308256 ingredient_slicer-0.0.88/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.309883 ingredient_slicer-0.0.88/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.88/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.88/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.88/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.88/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-18 12:58:21.331833 ingredient_slicer-0.0.88/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-0.0.88/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.312194 ingredient_slicer-0.0.88/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1593 2024-04-12 23:01:01.000000 ingredient_slicer-0.0.88/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   153828 2024-04-17 00:07:16.000000 ingredient_slicer-0.0.88/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   101598 2024-04-13 21:23:22.000000 ingredient_slicer-0.0.88/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-0.0.88/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    94843 2024-04-18 00:54:35.000000 ingredient_slicer-0.0.88/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.331194 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2021 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-11 13:20:33.000000 ingredient_slicer-0.0.88/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-18 12:58:21.332143 ingredient_slicer-0.0.88/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.330835 ingredient_slicer-0.0.88/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.88/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.88/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-0.0.88/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.88/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.88/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.88/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.88/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.88/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.88/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.88/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.88/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.88/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.88/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.88/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.88/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.88/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.88/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.88/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.88/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.88/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.88/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-0.0.88/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.88/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.88/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.88/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.88/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.88/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.88/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.88/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.88/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.88/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.88/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.88/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.88/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.88/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.88/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.88/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.88/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.653362 ingredient_slicer-1.0.0/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.631990 ingredient_slicer-1.0.0/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.633497 ingredient_slicer-1.0.0/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.0/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.0/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.0/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-07 12:26:18.653073 ingredient_slicer-1.0.0/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.0/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.636817 ingredient_slicer-1.0.0/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-06 13:28:44.000000 ingredient_slicer-1.0.0/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   155546 2024-05-06 15:43:05.000000 ingredient_slicer-1.0.0/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.0/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.0/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   101437 2024-05-06 17:10:27.000000 ingredient_slicer-1.0.0/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.652385 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2070 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-06 13:29:01.000000 ingredient_slicer-1.0.0/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-07 12:26:18.653430 ingredient_slicer-1.0.0/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.652019 ingredient_slicer-1.0.0/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.0/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.0/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.0/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.0/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.0/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.0/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.0/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.0/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.0/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.0/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.0/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.0/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.0/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.0/tests/test_get_single_item_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_gram_weights.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.0/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.0/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.0/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.0/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.0/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.0/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.0/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.0/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.0/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.0/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.0/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.0/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.0/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.0/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.0/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.0/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.0/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.0/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.0/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.0/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.0/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.0/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.0/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.0/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.0/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-0.0.88/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-1.0.0/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/.gitignore` & `ingredient_slicer-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/LICENSE` & `ingredient_slicer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/PKG-INFO` & `ingredient_slicer-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.88
+Version: 1.0.0
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-0.0.88/README.md` & `ingredient_slicer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer/__init__.py` & `ingredient_slicer-1.0.0/ingredient_slicer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # __init__.py
 
-__version__ = "0.0.88"
+__version__ = "1.0.0"
+
+from ._ingredient_slicer import IngredientSlicer
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
-    PRIMARY_CATEGORIES, SECONDARY_CATEGORIES
+    PRIMARY_CATEGORIES, SECONDARY_CATEGORIES, \
+    GRAM_CONVERSION_FACTORS, MILLILITER_CONVERSION_FACTORS \
 
-from ._ingredient_slicer import IngredientSlicer
 # from ._regex_patterns import IngredientTools
 # from ._utils import _make_int_or_float_str, _fraction_str_to_decimal, \
 #     _find_substring_indices, _find_and_remove_hyphens_around_substring
     # _replace_and_with_hyphen, _replace_to_or_with_hyphen, _replace_to_with_hyphen, _replace_or_with_hyphen
 
 
 __all__ = [
@@ -24,14 +26,16 @@
     "CASUAL_QUANTITIES",
     "PREP_WORDS",
     "FOOD_CATALOG",
     "FOOD_CATEGORIES",
     "FOOD_DENSITY_BY_GROUP",
     "PRIMARY_CATEGORIES",
     "SECONDARY_CATEGORIES",
+    "GRAM_CONVERSION_FACTORS",
+    "MILLILITER_CONVERSION_FACTORS",
     # Main parser classe
     'IngredientSlicer'
     # 'IngredientTools',  # Old regex patterns class
     ]
 
 # # ---- OLD Constants ----
 # 'NUMBER_WORDS',
```

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer/_constants.py` & `ingredient_slicer-1.0.0/ingredient_slicer/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1883,14 +1883,19 @@
             "pinot noir": ("wine_and_cider", "wine"),
             "chardonnay": ("wine_and_cider", "wine"),
             "sauvignon blanc": ("wine_and_cider", "wine"),
             "merlot": ("wine_and_cider", "wine"),
             "cabernet sauvignon": ("wine_and_cider", "wine"),
             "rosé": ("wine_and_cider", "wine"),
             "rose": ("wine_and_cider", "wine"),
+            "ruby port": ("wine_and_cider", "wine"),
+            "tawny port": ("wine_and_cider", "wine"),
+            "port": ("wine_and_cider", "wine"),
+            "ports": ("wine_and_cider", "wine"),
+            "port wine": ("wine_and_cider", "wine"),
             "rose wine" : ("wine_and_cider", "wine"),
             "champagne": ("wine_and_cider", "wine"),
             "sparkling wine": ("wine_and_cider", "wine"),
             "dessert wine": ("wine_and_cider", "wine"),
             "cooking wine": ("wine_and_cider", "wine"),
 
             # -------------------------------------------------------------------------------------------------------
@@ -2376,23 +2381,82 @@
     "eggs" : "egg_and_egg_products",
     "wine" : "wine_and_cider",
     "wines" : "wine_and_cider",
     "beer" : "beer",
     "beers" : "beer"
 }
 
-# # Categories that indicators point to:
-# cereal_and_cereal_products
-# egg_and_egg_products
-# oils 
-# milk
-# syrups
-# sweets
-# wine_and_cider
-# beer
+# A map of common food items and their weight in grams (i.e. 1 egg is approximately 56.7 grams, 1 apple is approximately 195 grams, etc.)
+SINGLE_ITEM_FOOD_WEIGHTS = {
+    'egg': '56.7',
+    'apple': '195',
+    'apricot': '35',
+    'avocado': '170',
+    'banana': '120',
+    'blackberry': '2.45',
+    'blueberry': '0.5',
+    'cherries': '5',
+    'coconut': '680',
+    'cranberry': '1.13',
+    'fig': '50',
+    'grapefruit': '246',
+    'grapes': '5',
+    'guava': '200',
+    'jackfruit': '6800',
+    'durian': '6800',
+    'kiwi': '75',
+    'lemon': '100',
+    'lime': '50',
+    'mango': '200',
+    'cantaloupe': '1360',
+    'honeydew': '1800',
+    'melon': '1500',
+    'nectarine': '150',
+    'olives': '5',
+    'orange': '130',
+    'papaya': '450',
+    'peach': '150',
+    'pear': '180',
+    'pineapple': '1590',
+    'plum': '65',
+    'pomegranate': '255',
+    'pumpkin': '4500',
+    'raspberry': '5',
+    'strawberry': '12',
+    'watermelon': '9000',
+    'artichoke': '368',
+    'asparagus': '22',
+    'eggplant': '453.5',
+    'garlic': '5',
+    'green beans': '5',
+    'beets': '113',
+    'bell pepper': '170',
+    'broccoli': '225',
+    'brussel sprouts': '14',
+    'cabbage': '9070',
+    'carrots': '60',
+    'cauliflower': '500',
+    'celery': '450',
+    'corn': '180',
+    'cucumber': '250',
+    'kale': '198',
+    'lettuce': '650',
+    'mushrooms': '15',
+    'onion': '160',
+    'parsnip': '115',
+    'pea': '0.2',
+    'potato': '184',
+    'snow pea': '2.5',
+    'spinach': '30',
+    'squash': '200',
+    'butternut squash': '1100',
+    'sweet potato': '113',
+    'tomato': '170',
+    'zucchini': '200'
+}
 
 # ----------------------------------------------------------------------------
 # ---- Unused constants ----
 # ----------------------------------------------------------------------------
 
 # TODO: Probably can delete the constants below, they've been replaced/deprecated by other constants
```

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-1.0.0/ingredient_slicer/_ingredient_slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._standardized_unit = None   # "standard units" are the commonplace names for the found units (i.e. the standard unit of "oz" is "ounce")
         
         # make member variables for seconday quantities and units
         self._secondary_quantity = None
         self._secondary_unit     = None
         self._standardized_secondary_unit = None
 
-        self._gram_weight          = None
+        self._gram_weight         = None
         self._min_gram_weight     = None
         self._max_gram_weight     = None
 
         # "prep" are words that describe the state of the ingredient (i.e. "chopped", "diced", "minced")
         self._prep                  = []
 
         # "size modifiers" are words that describe the size of the ingredient (i.e. "large", "small", "medium")
@@ -1613,20 +1613,35 @@
     
     def _add_gram_weights(self):
         """Add gram weights to the units variables if they are the only possible units after the ingredient has been parsed."""
         # ingredient = "2 1/2 cups of sugar (about 1/2 inch squares of sugar)"
         grams_map = _utils._get_gram_weight(self._food, self._quantity, self._unit, "dice")
 
         if grams_map:
-            self._gram_weight      = grams_map.get("gram_weight", None)
+            self._gram_weight     = grams_map.get("gram_weight", None)
             self._min_gram_weight = grams_map.get("min_gram_weight", None)
             self._max_gram_weight = grams_map.get("max_gram_weight", None)
 
         return
+    
+    def _add_gram_weights_for_single_item_foods(self):
+
+        if not self._gram_weight:
+
+            # print(f'THIS IS A SINGLE ITEM FOOD: {self._food}') if self.debug else None
+            # NOTE: this is an arbitrary fuzzy string matching ratio of 0.5 for now
+            gram_weight = _utils._get_single_item_gram_weight(self._food, self._quantity, 0.5)
+            
+            # print(f" >>> Gram weight for single item food: {gram_weight}") if self.debug else None
+            
+            self._gram_weight = gram_weight
 
+        return 
+
+    
     def _address_parenthesis(self) -> None:
         """
         Address any parenthesis that were in the ingredient.
         """
         # print(f"Addressing parenthesis: '{self._parenthesis_content}'") if self.debug else None
 
         # loop through each of the parenthesis in the parenthesis content and apply address_parenthesis functions 
@@ -1730,14 +1745,20 @@
 
         # ----------------------------------- STEP 9 ------------------------------------------
         # ---- Calculate gram weights if possible ----
         # -------------------------------------------------------------------------------------
         print(f"Calculating gram weights") if self.debug else None
         self._add_gram_weights() # TODO: testing using staged_ingredient
 
+        # ----------------------------------- STEP 10 ------------------------------------------
+        # ---- Calculate gram weights if possible ----
+        # -------------------------------------------------------------------------------------
+        print(f"Estimating gram weights for unitless foods") if self.debug else None
+        self._add_gram_weights_for_single_item_foods() # TODO: testing using staged_ingredient
+
 
     def standardized_ingredient(self) -> str:
         """
         Return the standardized ingredient string.
         Returns:
             str: The standardized ingredient string.
         """
```

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-1.0.0/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer/_utils.py` & `ingredient_slicer-1.0.0/ingredient_slicer/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,18 +317,14 @@
             ingredient (str): The ingredient string to update
             pattern (re.Pattern): The pattern to use to find the ranges
         Returns:
             str: The updated ingredient string with all possible ranges updated to always 
                 have 2 numbers separated by a whitespace, then a hyphen, then another whitespace.
         """
 
-        # # pattern = IngredientSlicer.regex.QUANTITY_DASH_QUANTITY
-        # ingredient = "1-2 apples and 1- 45 orange slices between 4 and 5 lemons or 1 or 2 oranges and use 1 to 2 lemons"
-        # pattern = _regex_patterns.QUANTITY_DASH_QUANTITY
-        
         matched_ranges_iter = pattern.finditer(ingredient)
         offset = 0
 
         for match in matched_ranges_iter:
             start, end = match.start(), match.end()
             modified_start = start + offset  # new start position
             modified_end = end + offset      # new end position
@@ -623,30 +619,14 @@
     """Remove extra whitespaces from a string and return the string with only single whitespaces."""
     # ingredient = re.sub(r'\s+', ' ', ingredient).strip() # remove any extra whitespace
     return " ".join(input_string.split())
 
 # -----------------------------------------------------------------------------------------------
 # ---- Functions for parsing parenthesis content / quantity unit regex functions ----
 # -----------------------------------------------------------------------------------------------
-
-# def test_parenthesis_with_equiv_quantity_unit_1():
-#     parse = IngredientSlicer("1 cup of chopped chicken breast (about 12 ounces)", debug = True)
-#     # parse.parse()
-#     parsed = parse.to_json()
-
-#     assert parsed['quantity'] == "12"
-#     assert parsed['unit'] == "ounces"
-#     assert parsed["standardized_unit"] == "ounce"
-
-#     assert parsed['secondary_quantity'] == None  # TODO: maybe this case should get a quantity of 1, but for now it's None
-#     assert parsed['secondary_unit'] == "breast"
-#     assert parsed['standardized_secondary_unit'] == "breast"
-
-#     assert parsed['is_required'] == True
-
 def _extract_quantities_only(input_string: str) -> list:
 
     """From a string get all quantities if they exist WITHOUT units
     Useful for just getting quantities if there are no units associated with them (e.g. "chicken breast (5)")
     Args:
         input_string (str): The string to parse
     Returns:
@@ -730,17 +710,15 @@
 
     Args:
         input_string (str): The string to parse
     Returns:
         list: A list of tuples containing the (approximate string, quantity, and unit)
     """
 
-    # input_string = parenthesis
     # input_string = '(about 12 tender and juicy ounces or about 14 grams)'
-    # input_string = '(juicy about or 14)'
     # input_string = '(12 tender and juicy ounces or 14 grams about)'
 
     if not isinstance(input_string, str):
         raise ValueError("Invalid input. Input must be a string.")
 
     # regex_patterns = _regex_patterns.IngredientTools()
 
@@ -1428,21 +1406,14 @@
     Examples:
         >>> _removed_x_separators("1x2 cups")
         '1 2 cups'
         >>> _remove_x_separators("5 x cartons of eggs")
         "5   cartons of eggs"
     """
     # ingredient = "5 x cartons of eggs (3 x 4 inches)"
-    # # ingredient = "4x 4  inch"
-    # _regex_patterns.SINGLE_DIMENSION_UNIT_RANGES.findall(ingredient)
-    # _regex_patterns.X_AFTER_NUMBER.findall(ingredient)
-    # _regex_patterns.NUMBER_X_NUMBER.findall(ingredient)
-    # _regex_patterns.X_AFTER_NUMBER.findall("4x4inch")
-    # _regex_patterns.X_AFTER_NUMBER.findall("4x4 inch")
-    # _regex_patterns.X_AFTER_NUMBER.findall("4 x 4 inch")
 
     def replace_x(match):
         return match.group().replace('x', ' ').replace('X', ' ')
 
     # Replace "x"/"X" separators with whitespace
     ingredient = _regex_patterns.X_AFTER_NUMBER.sub(replace_x, ingredient)
 
@@ -1488,17 +1459,14 @@
     Args:
         food (str): The food item to convert.
         quantity (Union[str, int, float]): The quantity of the food item.
         unit (str): The unit of measurement for the quantity.
     Returns:
         dict: A dictionary containing the gram weight, maximum gram weight, and minimum gram weight.
     """
-    # food = "olive oil"
-    # quantity = "1"
-    # unit = "teaspoon"
 
     if not unit:
         return {
             "gram_weight" : None,
             "min_gram_weight" : None,
             "max_gram_weight" : None
         }
@@ -1517,45 +1485,60 @@
 
     if method not in ["levenshtein", "jaccard", "dice"]:
         raise ValueError("Invalid 'method'. Options are 'levenshtein', 'jaccard', or 'dice'.")
     
     if not isinstance(quantity, (str, int, float)):
         raise ValueError("'quantity' must be a string, integer, or float")
     
+    # if unit is not None and not isinstance(unit, str):
     if not isinstance(unit, str):
         raise ValueError("'unit' must be a string")
 
     quantity = float(quantity)
     
     gram_weight     = None
     min_gram_weight = None
     max_gram_weight = None
     
+    # if unit:
     unit = unit.lower()
+    
+    unit_is_weight = unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT
+    unit_is_volume = unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT
 
     # weight check
-    if unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT:
+    if unit_is_weight:
         gram_weight = _convert_weights_to_grams(quantity, unit)
 
         return {
             "gram_weight" : str(round(gram_weight, 2)) if gram_weight else None,
             "min_gram_weight" : str(round(min_gram_weight, 2)) if min_gram_weight else None,
             "max_gram_weight" : str(round(max_gram_weight, 2)) if max_gram_weight else None
             }
     
     # volume check
-    if unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT:
+    if unit_is_volume:
         gram_values_map = _convert_volume_to_grams(food, quantity, unit, method)  
 
         return {
             "gram_weight" : str(round(gram_values_map["gram_weight"], 2)) if gram_values_map["gram_weight"] else None,
             "min_gram_weight" : str(round(gram_values_map["min_gram_weight"], 2)) if gram_values_map["min_gram_weight"] else None,
             "max_gram_weight" : str(round(gram_values_map["max_gram_weight"], 2)) if gram_values_map["max_gram_weight"] else None
             }
 
+    # if not unit or unit is None or (not unit_is_weight and not unit_is_volume):
+    #     print(f"Attempting to get gram weights for single item...\n > food: '{food}'\n > quantity: '{quantity}'\n > unit: '{unit}'\n > gram_weight: '{gram_weight}'")
+    #     gram_weight = _get_single_item_gram_weight(food, quantity, unit, gram_weight)
+
+    #     return {
+    #         "gram_weight" : str(round(gram_weight, 2)) if gram_weight else None,
+    #         "min_gram_weight" : str(round(min_gram_weight, 2)) if min_gram_weight else None,
+    #         "max_gram_weight" : str(round(max_gram_weight, 2)) if max_gram_weight else None
+    #         }
+
     # if the given unit was not a weight or volume unit, return None for all of the gram weights
     return {
         "gram_weight" : str(round(gram_weight, 2)) if gram_weight else None,
         "min_gram_weight" : str(round(min_gram_weight, 2)) if min_gram_weight else None,
         "max_gram_weight" : str(round(max_gram_weight, 2)) if max_gram_weight else None
         }
     
@@ -1914,14 +1897,218 @@
     first_bigrams = {first[i : i + 2] for i in range(len(first) - 1)}
     second_bigrams = {second[i : i + 2] for i in range(len(second) - 1)}
 
     intersection = first_bigrams & second_bigrams
 
     return 2.0 * len(intersection) / (len(first_bigrams) + len(second_bigrams))
 
+def _fuzzy_match_key(fuzzy_key:str = None, 
+                    map_to_check:dict = _constants.FOOD_CATEGORIES, 
+                    method:str = "dice",
+                    threshold: Union[float, None] = None,
+                    ) -> str:
+    """
+    Get the key from the map that most closely matches the fuzzy key
+    Args:
+    fuzzy_key: key to match
+    map_to_check: dictionary to check for matches
+    method: method to use for fuzzy matching. Options are "dice", "jaccard", or "levenshtein"
+    threshold: minimum similarity score to return a match (between 0 and 1, default is None)
+    """
+
+    if threshold is not None and not isinstance(threshold, float):
+        raise ValueError("Threshold must be a float")
+
+    method = method.lower()
+
+    if method not in ["dice", "jaccard", "levenshtein"]:
+        raise ValueError("Invalid method. Options are 'dice', 'jaccard', or 'levenshtein'")
+
+    # fuzzy_key = primary_categories[0]
+    # map_to_check = ingredient_slicer.FOOD_CATEGORIES
+
+    fuzzy_matcher = _get_fuzzy_matcher(method)
+    # map_keys = list(map_to_check.keys())
+
+    best_match = None
+    max_similarity = 0
+    
+    for key in map_to_check.keys():
+        similarity = round(fuzzy_matcher(fuzzy_key, key), 3)
+
+        if similarity >= max_similarity:
+            max_similarity = similarity
+            best_match = key
+    
+    if threshold and max_similarity < threshold:
+        return None
+    
+    return best_match
+
+def _fuzzy_match_str_parts_to_key(fuzzy_key:str = None, 
+                    map_to_check:dict = _constants.FOOD_CATEGORIES, 
+                    method:str = "dice",
+                    threshold: Union[float, None] = None,
+                    ) -> str:
+    """
+    Get the key from the map that most closely matches the fuzzy key
+    Args:
+    fuzzy_key: key to match, the key is split into parts and each part is matched to the map keys
+    map_to_check: dictionary to check for matches
+    method: method to use for fuzzy matching. Options are "dice", "jaccard", or "levenshtein"
+    threshold: minimum similarity score to return a match (between 0 and 1, default is None)
+    Returns:
+        str: The key that most closely matches the fuzzy key
+    """
+    # fuzzy_key = 'farmraised fresh eggs'
+    # fuzzy_key = "fresh broccoli heads, light"
+    # map_to_check = _constants.SINGLE_ITEM_FOOD_WEIGHTS
+    # method = "dice"
+    # threshold = None
+
+    if threshold is not None and not isinstance(threshold, float):
+        raise ValueError("Threshold must be a float")
+
+    method = method.lower()
+
+    if method not in ["dice", "jaccard", "levenshtein"]:
+        raise ValueError("Invalid method. Options are 'dice', 'jaccard', or 'levenshtein'")
+
+    # fuzzy_key = primary_categories[0]
+    # map_to_check = ingredient_slicer.FOOD_CATEGORIES
+
+    fuzzy_matcher = _get_fuzzy_matcher(method)
+    # map_keys = list(map_to_check.keys())
+
+    best_match = None
+    max_similarity = 0
+
+    split_fuzzy_key = fuzzy_key.split()
+    
+    for key in map_to_check.keys():
+        split_max_score = 0
+        for split_fuzzy in split_fuzzy_key:
+            # print(f"Split Fuzzy: {split_fuzzy}")
+            if split_fuzzy == key:
+                max_similarity = 1
+                best_match = key
+                continue
+
+            similarity = round(fuzzy_matcher(split_fuzzy, key), 3)
+            # print(f"Split Fuzzy: {split_fuzzy} > '{similarity}")
+
+            split_max_score = max(similarity, split_max_score)
+            # split_scores.append(similarity)
+            # split_max_score = max(split_scores)
+        
+        if split_max_score >= max_similarity:
+            # print(f"New best match: {key}")
+            max_similarity = split_max_score
+            best_match = key
+
+        # print(f"best_match: {best_match}")
+        # print(f"max_similarity: {max_similarity}")
+        # print()
+
+    if threshold and max_similarity < threshold:
+        # print(f"Best match WAS '{best_match}' but the similarity score was too low ({max_similarity} < {threshold})")
+        return None
+    
+    # print(f"Best match is '{best_match}' with a similarity score of {max_similarity}")
+    return best_match
+
+def _estimate_single_item_gram_weights(food:str, threshold:Union[float, None]) -> Union[str, None]:
+
+    """ Estimate the weight of a single food item in grams
+    Args:
+        food: str, food item
+        threshold: float, minimum similarity score to return a match
+    Returns:
+        estimated weight of the food in grams as a string or None
+    """
+
+    # food = "egg whites"
+    # gram_weight = None
+
+    # if gram_weight or gram_weight is not None:
+    #     return gram_weight
+    
+    if food in _constants.SINGLE_ITEM_FOOD_WEIGHTS:
+        return _constants.SINGLE_ITEM_FOOD_WEIGHTS[food]
+    
+    # closest_key = _fuzzy_match_key(food, _constants.SINGLE_ITEM_FOOD_WEIGHTS, "dice", 0.5)
+    closest_key = _fuzzy_match_str_parts_to_key(food, _constants.SINGLE_ITEM_FOOD_WEIGHTS, "dice", threshold)
+
+    # if closest_key:
+        # return _constants.SINGLE_ITEM_FOOD_WEIGHTS[closest_key]
+    
+    return _constants.SINGLE_ITEM_FOOD_WEIGHTS.get(closest_key, None)
+
+def _get_single_item_gram_weight2(food:str, quantity:str, unit:str, gram_weight:str) -> Union[str, None]:
+
+    """ Get the weight of a single food item in grams
+    Args:
+        food: str, food item
+        quantity: str, quantity of the food item
+        unit: str, unit of measurement for the quantity
+        gram_weight: str, weight of the food in grams
+
+    Returns:
+        estimated weight of the food in grams as a string or None
+    """
+
+    # food = "eggs"
+    # unit = "cup"
+    # unit = None
+    # quantity = 1
+    # gram_weight = None
+    
+    # set quantity to 1 if its None
+    quantity = 1 if not quantity else float(quantity)
+
+    # gram_weight already exists or the unit is a weight unit or volume unit just return the gram weight
+    # if gram_weight or unit in _constants.BASIC_UNITS_SET or unit in _constants.VOLUME_UNITS_SET:
+    if gram_weight or unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT or unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT:
+        return gram_weight
+    
+    est_weight = _estimate_single_item_gram_weights(food)
+    
+    return float(est_weight) * quantity if est_weight else None
+
+def _get_single_item_gram_weight(food:str, quantity:str, threshold:Union[float, None] = None) -> Union[str, None]:
+
+    """ Get the weight of a single food item in grams
+    Args:
+        food: str, food item
+        quantity: str, quantity of the food item
+
+    Returns:
+        estimated weight of the food in grams as a string or None
+    """
+
+    if not isinstance(food, str):
+        raise TypeError("'food' must be a string")
+    
+    if quantity is not None and not isinstance(quantity, (str, int, float)):
+        raise TypeError("'quantity' must be a string, integer, or float")
+
+    # food = "eggs"
+    # unit = "cup"
+    # unit = None
+    # quantity = 1
+    # gram_weight = None
+    
+    # set quantity to 1 if its None
+    quantity = 1 if not quantity else float(quantity)
+    
+    est_weight = _estimate_single_item_gram_weights(food,  threshold)
+    
+    return str(float(est_weight) * quantity) if est_weight else None
+
+
 # def _split_dimension_unit_x_ranges(ingredient: str) -> tuple[str]:
 #     """Split an ingredient string by any quantity dimension unit separated by an 'x' character.
 #     (i.e. "2 steaks, 3 inches x 4 inches thick" -> ("2 steaks, thick", "3 inches x 4 inches")
 
 #     Args:
 #         ingredient (str): The ingredient string to parse.
 #     Returns:
```

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-1.0.0/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.88
+Version: 1.0.0
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-0.0.88/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-1.0.0/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
-.github/workflows/publish-to-pypi.yml
 .github/workflows/run-unit-tests.yml
 ingredient_slicer/__init__.py
 ingredient_slicer/_constants.py
 ingredient_slicer/_ingredient_slicer.py
 ingredient_slicer/_regex_patterns.py
 ingredient_slicer/_utils.py
 ingredient_slicer.egg-info/PKG-INFO
@@ -23,17 +22,19 @@
 tests/test_duplicate_unit_ranges.py
 tests/test_extract_dimensions.py
 tests/test_extract_quantities_utils.py
 tests/test_find_and_remove.py
 tests/test_find_and_remove_hyphen_substrings.py
 tests/test_fraction_str_to_decimal.py
 tests/test_get_gram_weight.py
+tests/test_get_single_item_gram_weight.py
 tests/test_ingredient_slicer.py
 tests/test_ingredient_slicer_dimensions.py
 tests/test_ingredient_slicer_fraction_conversions.py
+tests/test_ingredient_slicer_gram_weights.py
 tests/test_ingredient_slicer_parenthesis.py
 tests/test_ingredient_slicer_x_separators.py
 tests/test_is_approximate_quantity_only_parenthesis.py
 tests/test_make_int_or_float_str.py
 tests/test_merge_misleading_ranges.py
 tests/test_merge_numbers.py
 tests/test_number_ranges.py
```

### Comparing `ingredient_slicer-0.0.88/pyproject.toml` & `ingredient_slicer-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "0.0.88"
+version = "1.0.0"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-0.0.88/tests/test_avg_ranges.py` & `ingredient_slicer-1.0.0/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_casual_ingredients.py` & `ingredient_slicer-1.0.0/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-1.0.0/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-1.0.0/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-1.0.0/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_extract_dimensions.py` & `ingredient_slicer-1.0.0/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_extract_quantities_utils.py` & `ingredient_slicer-1.0.0/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_find_and_remove.py` & `ingredient_slicer-1.0.0/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-1.0.0/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-1.0.0/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_get_gram_weight.py` & `ingredient_slicer-1.0.0/tests/test_get_gram_weight.py`

 * *Files 4% similar despite different names*

```diff
@@ -493,12 +493,26 @@
     assert min_gram_weight is None
     assert max_gram_weight is None
     
 def test_get_gram_weight_fraction_as_quantity():
     with pytest.raises(ValueError):
         _utils._get_gram_weight("olive oil", "1/2", "teaspoon")
 
+# TODO: Need to refine behavior for foods that dont have a real unit or any unit at all
+# TODO: Reference the _get_single_item_gram_weight() function that tries to take a food with no weight or volume unit 
+# TODO: and get the gram weight. _get_single_item_gram_weight() assumes that if a food has no unit and or a Non weight/volume unit (i.e. 'heads') than the ingredient 
+# TODO: is an individual item type ingredient where the food is also the unit (i.e. 2 eggs). There is a small/hacky SINGLE_ITEM_FOOD_WEIGHTS dictionary 
+# TODO:  with an average gram weight of some common single item foods (primarly fruits, vegetables, and eggs)
 def test_get_gram_weight_invalid_unit():
     assert _utils._get_gram_weight("olive oil", "1", "fgdhdjgfhdf") == {"gram_weight": None, 
                                                                  "min_gram_weight": None, 
                                                                  "max_gram_weight": None}
     
+# def test_get_gram_weight_one_egg_no_unit():
+#     assert _utils._get_gram_weight("egg", "1", None) == {"gram_weight": '56.7', 
+#                                                                  "min_gram_weight": None, 
+#                                                                  "max_gram_weight": None}
+    
+# def test_get_gram_weight_two_eggs_no_unit():
+#     assert _utils._get_gram_weight("egg", "2", None) == {"gram_weight": '113.4', 
+#                                                                  "min_gram_weight": None, 
+#                                                                  "max_gram_weight": None}
```

### Comparing `ingredient_slicer-0.0.88/tests/test_ingredient_slicer.py` & `ingredient_slicer-1.0.0/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-1.0.0/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_make_int_or_float_str.py` & `ingredient_slicer-1.0.0/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-1.0.0/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_merge_numbers.py` & `ingredient_slicer-1.0.0/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_number_ranges.py` & `ingredient_slicer-1.0.0/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-1.0.0/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-1.0.0/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_parenthesis.py` & `ingredient_slicer-1.0.0/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_parenthesis_utils.py` & `ingredient_slicer-1.0.0/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_percentages.py` & `ingredient_slicer-1.0.0/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-1.0.0/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_prep_words.py` & `ingredient_slicer-1.0.0/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_quantity_range_regex.py` & `ingredient_slicer-1.0.0/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_quantity_units_regex.py` & `ingredient_slicer-1.0.0/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-1.0.0/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_remove_x_separators.py` & `ingredient_slicer-1.0.0/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-1.0.0/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_separate_dimensions.py` & `ingredient_slicer-1.0.0/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_size_modifiers.py` & `ingredient_slicer-1.0.0/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_spaced_numbers.py` & `ingredient_slicer-1.0.0/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_unit_regex.py` & `ingredient_slicer-1.0.0/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_wild_ingredients.py` & `ingredient_slicer-1.0.0/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_word_fractions.py` & `ingredient_slicer-1.0.0/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_word_numbers.py` & `ingredient_slicer-1.0.0/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.88/tests/test_x_after_number_regex.py` & `ingredient_slicer-1.0.0/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

