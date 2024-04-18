# Comparing `tmp/ingredient_slicer-0.0.87.tar.gz` & `tmp/ingredient_slicer-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-0.0.87.tar", last modified: Wed Apr 10 14:54:57 2024, max compression
+gzip compressed data, was "ingredient_slicer-0.0.88.tar", last modified: Thu Apr 18 12:58:21 2024, max compression
```

## Comparing `ingredient_slicer-0.0.87.tar` & `ingredient_slicer-0.0.88.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.647555 ingredient_slicer-0.0.87/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.634620 ingredient_slicer-0.0.87/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.636262 ingredient_slicer-0.0.87/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.87/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.87/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.87/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.87/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-10 14:54:57.647269 ingredient_slicer-0.0.87/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-0.0.87/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.637438 ingredient_slicer-0.0.87/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-10 14:53:27.000000 ingredient_slicer-0.0.87/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   155518 2024-04-10 14:53:06.000000 ingredient_slicer-0.0.87/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   105302 2024-04-10 14:53:09.000000 ingredient_slicer-0.0.87/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-10 14:53:09.000000 ingredient_slicer-0.0.87/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    98187 2024-04-10 14:53:05.000000 ingredient_slicer-0.0.87/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.646577 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2021 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-10 14:54:41.000000 ingredient_slicer-0.0.87/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-10 14:54:57.647611 ingredient_slicer-0.0.87/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.646342 ingredient_slicer-0.0.87/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.87/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.87/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-0.0.87/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.87/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.87/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.87/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.87/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.87/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.87/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.87/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.87/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.87/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.87/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.87/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.87/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.87/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.87/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.87/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.87/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.87/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-0.0.87/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.87/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.87/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.87/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.87/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.87/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.87/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.87/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.87/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.87/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.87/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.87/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.87/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.87/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.87/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.87/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.332093 ingredient_slicer-0.0.88/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.308256 ingredient_slicer-0.0.88/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.309883 ingredient_slicer-0.0.88/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.88/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.88/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.88/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.88/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-18 12:58:21.331833 ingredient_slicer-0.0.88/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-0.0.88/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.312194 ingredient_slicer-0.0.88/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1593 2024-04-12 23:01:01.000000 ingredient_slicer-0.0.88/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   153828 2024-04-17 00:07:16.000000 ingredient_slicer-0.0.88/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   101598 2024-04-13 21:23:22.000000 ingredient_slicer-0.0.88/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-0.0.88/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    94843 2024-04-18 00:54:35.000000 ingredient_slicer-0.0.88/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.331194 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2021 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-18 12:58:21.000000 ingredient_slicer-0.0.88/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-11 13:20:33.000000 ingredient_slicer-0.0.88/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-18 12:58:21.332143 ingredient_slicer-0.0.88/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-18 12:58:21.330835 ingredient_slicer-0.0.88/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.88/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.88/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-0.0.88/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.88/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.88/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.88/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.88/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.88/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.88/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.88/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.88/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.88/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.88/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.88/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.88/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.88/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.88/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.88/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.88/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.88/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.88/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.88/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-0.0.88/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.88/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.88/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.88/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.88/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.88/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.88/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.88/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.88/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.88/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.88/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.88/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.88/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.88/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.88/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.88/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.88/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-0.0.87/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-0.0.88/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-0.0.88/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/.gitignore` & `ingredient_slicer-0.0.88/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/LICENSE` & `ingredient_slicer-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/PKG-INFO` & `ingredient_slicer-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.87
+Version: 0.0.88
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-0.0.87/README.md` & `ingredient_slicer-0.0.88/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer/__init__.py` & `ingredient_slicer-0.0.88/ingredient_slicer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # __init__.py
 
-__version__ = "0.0.87"
+__version__ = "0.0.88"
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
-    FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP
+    FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
+    PRIMARY_CATEGORIES, SECONDARY_CATEGORIES
 
 from ._ingredient_slicer import IngredientSlicer
 # from ._regex_patterns import IngredientTools
 # from ._utils import _make_int_or_float_str, _fraction_str_to_decimal, \
 #     _find_substring_indices, _find_and_remove_hyphens_around_substring
     # _replace_and_with_hyphen, _replace_to_or_with_hyphen, _replace_to_with_hyphen, _replace_or_with_hyphen
 
@@ -21,14 +22,16 @@
     "DIMENSION_UNITS", 
     "CASUAL_UNITS", 
     "CASUAL_QUANTITIES",
     "PREP_WORDS",
     "FOOD_CATALOG",
     "FOOD_CATEGORIES",
     "FOOD_DENSITY_BY_GROUP",
+    "PRIMARY_CATEGORIES",
+    "SECONDARY_CATEGORIES",
     # Main parser classe
     'IngredientSlicer'
     # 'IngredientTools',  # Old regex patterns class
     ]
 
 # # ---- OLD Constants ----
 # 'NUMBER_WORDS',
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer/_constants.py` & `ingredient_slicer-0.0.88/ingredient_slicer/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -2147,22 +2147,22 @@
         FOODS_BY_CATEGORY[primary_category] = set([key])
 
     if secondary_category in FOODS_BY_CATEGORY:
         FOODS_BY_CATEGORY[secondary_category].add(key)
     else: 
         FOODS_BY_CATEGORY[secondary_category] = set([key])
 
-# FOODS_BY_CATEGORY = {}
-# for key, val in FOOD_CATALOG.items():
-#     current_major_set = FOODS_BY_CATEGORY.get(primary_category, set())
-#     current_minor_set = FOODS_BY_CATEGORY.get(secondary_category, set())
-#     current_major_set.add(key)
-#     current_minor_set.add(key)
-#     FOODS_BY_CATEGORY[primary_category] = current_major_set
-#     FOODS_BY_CATEGORY[secondary_category] = current_minor_set
+PRIMARY_CATEGORIES = tuple(FOOD_CATEGORIES.keys())
+
+SECONDARY_CATEGORIES = set()
+for key, value in FOOD_CATEGORIES.items():
+    for val in value:
+        SECONDARY_CATEGORIES.add(val)
+
+SECONDARY_CATEGORIES = tuple(SECONDARY_CATEGORIES)
 
 # -----------------------------------------------------------------------------------------------------
 # ---- Approximate food densities for food groups ----
 # -----------------------------------------------------------------------------------------------------
 
 # Specific food densities derived from the FAO/INFOODS Density Database version 2.0 (2012). 
 # The following categories are derived values for each group in the Density Database table
@@ -2353,23 +2353,14 @@
     "aerated": 0.5
 }
 
 # ----------------------------------------------------------------------------
 # ---- Strings that obviously point to a food being a specific category ----
 # ----------------------------------------------------------------------------
 
-# INDICATES_A_CEREAL = {"flour", "flours", "bread", "breads"}
-# INDICATES_AN_OIL   = {"oil", "oils"}
-# INDICATES_A_MILK   = {"milk", "milks"}
-# INDICATES_A_SYRUP  = {"syrup", "syrups"}
-# INDICATES_A_SUGAR  = {"sugar", "sugars"}
-# INDICATES_AN_EGG   = {"egg", "eggs"}
-# INDICATES_A_WINE   = {"wine", "wines"}
-# INDICATES_A_BEER   = {"beer", "beers"}
-
 # Words that are so obviously pointing to a specific category that they can be used to determine the category of a food
 # (i.e. if a food contains the word "flour", it is most likely a cereal product)
 INDICATOR_STRINGS_MAP = {
     "flour" : "cereal_and_cereal_products",
     "flours" : "cereal_and_cereal_products",
     "bread" : "cereal_and_cereal_products",
     "breads" : "cereal_and_cereal_products",
@@ -2394,14 +2385,15 @@
 # egg_and_egg_products
 # oils 
 # milk
 # syrups
 # sweets
 # wine_and_cider
 # beer
+
 # ----------------------------------------------------------------------------
 # ---- Unused constants ----
 # ----------------------------------------------------------------------------
 
 # TODO: Probably can delete the constants below, they've been replaced/deprecated by other constants
 
 # Fractions words representing the denominator of a fraction
@@ -2996,62 +2988,20 @@
 #     'Amaranth flour': {'volume': '1 cup', 'ounces': 3.625, 'grams': 103},
 #     'Apple juice concentrate': {'volume': '1/4 cup', 'ounces': 2.5, 'grams': 70}
 #     }
 # TODO: Code to simplify the above FOOD_CONVERSION_FACTORS dictionary
 # for key, value in FOOD_CONVERSION_FACTORS.items():
 #     volume_string = FOOD_CONVERSION_FACTORS[key]['volume']
 #     parsed_ingredient = IngredientSlicer(volume_string).to_json()
-
 #     quantity = float(parsed_ingredient['quantity'])
 #     unit = parsed_ingredient['unit']
-
 #     multiplication_factor = 1/quantity
-    
 #     converted_ounces = FOOD_CONVERSION_FACTORS[key]["ounces"] * multiplication_factor
 #     converted_grams  = FOOD_CONVERSION_FACTORS[key]["grams"] * multiplication_factor
 #     converted_volume = quantity * multiplication_factor
 
 #     FOOD_CONVERSION_FACTORS[key] = {
 #         'volume_quantity' : converted_volume,
 #         'volume_unit': unit,
 #         'ounces': converted_ounces, 
 #         'grams': converted_grams
-#     }
-# ---------------------------------------
-# ---- Old IngredientConstants class ----
-# ---------------------------------------
-
-# class IngredientConstants:
-
-#     # Primary unit maps
-#     UNITS = UNITS
-#     BASIC_UNITS = BASIC_UNITS
-
-#     # other (specific) unit maps
-#     WEIGHT_UNITS = WEIGHT_UNITS
-#     DIMENSION_UNITS = DIMENSION_UNITS
-#     CASUAL_UNITS = CASUAL_UNITS
-#     CASUAL_QUANTITIES = CASUAL_QUANTITIES
-
-#     # primary unit sets
-#     UNITS_SET = UNITS_SET
-#     BASIC_UNITS_SET = BASIC_UNITS_SET
-#     NON_BASIC_UNITS_SET = NON_BASIC_UNITS_SET
-    
-#     # other (specific) units sets
-#     WEIGHT_UNITS_SET = WEIGHT_UNITS_SET
-#     DIMENSION_UNITS_SET = DIMENSION_UNITS_SET
-#     CASUAL_UNITS_SET = CASUAL_UNITS_SET
-#     CASUAL_QUANTITIES_SET = CASUAL_QUANTITIES_SET
-#     SIZE_MODIFIERS_SET = SIZE_MODIFIERS_SET
-
-#     # Misc. Sets
-#     PREP_WORDS = PREP_WORDS
-#     APPROXIMATE_STRINGS = APPROXIMATE_STRINGS
-#     UNIT_MODIFIERS = UNIT_MODIFIERS
-    
-#     # generic stop words for parsing 
-#     STOP_WORDS = STOP_WORDS
-
-#     # food catalog and food categories
-#     FOOD_CATALOG = FOOD_CATALOG
-#     FOOD_CATEGORIES = FOOD_CATEGORIES
+#     }
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-0.0.88/ingredient_slicer/_ingredient_slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2011,95 +2011,7 @@
 #         self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(merged_quantity) + self._standardized_ingredient[modified_end:]
 #         # ingredient = ingredient[:modified_start] + str(merged_quantity) + ingredient[modified_end:]
 
 #         # Update the offset for subsequent replacements
 #         offset += len(merged_quantity) - (end - start)
 #         replacement_index += 1
 #         # print(f" --> Output ingredient: \n > '{self._standardized_ingredient}'")
-
-# ####### Deprecated ####### 
-# def _parse_fractions(self):
-#     """
-#     Replace unicode and standard fractions with their decimal equivalents in the parsed ingredient.
-#     """
-#     # print("Parsing fractions")
-#     # regex.MULTI_PART_FRACTIONS_PATTERN
-#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN, self._standardized_ingredient)
-#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self._standardized_ingredient)
-
-#     # finditer() method
-#     fractions = re.finditer(_regex_patterns.MULTI_PART_FRACTIONS_PATTERN, self._standardized_ingredient)
-#     # fractions = re.finditer(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self._standardized_ingredient)
-
-#     # Replace fractions in the original string with their sum based on match indices
-#     # updated_ingredient = self._standardized_ingredient
-#     offset = 0
-
-#     for match in fractions:
-
-#         # keep track of the offset to adjust the index of the match
-#         start_index = match.start() + offset
-#         end_index = match.end() + offset
-#         matched_fraction = match.group()
-
-#         print(f"Matched Fraction: {matched_fraction}")
-#         # remove "and" and "&" from the matched fraction
-#         matched_fraction = matched_fraction.replace("and", " ").replace("&", " ")
-
-#         print(f"Matched Fraction after removing AND: {matched_fraction}")
-
-#         # Parse the matched fraction, make sure it's in the correct format, to be able to be summed
-#         parsed_fraction = self._parse_mixed_fraction(matched_fraction)
-
-#         print(f"Parsed Fraction: {parsed_fraction}")
-
-#         # Replace the matched fraction with the sum of the parse    d fraction
-#         sum_fraction = self._sum_parsed_fractions(parsed_fraction)
-
-#         print(f"Sum Fraction: {sum_fraction}")
-#         # Insert the sum of the fraction into the updated ingredient string
-#         # updated_ingredient = updated_ingredient[:start_index] + str(sum_fraction) + updated_ingredient[end_index:]
-#         self._standardized_ingredient = self._standardized_ingredient[:start_index] + " " + str(sum_fraction) + self._standardized_ingredient[end_index:]
-
-#         # Update the offset to account for the difference in length between the matched fraction and the sum of the fraction
-#         offset += len(str(sum_fraction)) - len(matched_fraction)
-
-# ####### Deprecated ####### 
-# def _parse_mixed_fraction(self, fraction_str: str) -> list:
-#     # Remove whitespace to the left and right of a slash
-#     cleaned_fractions = re.sub(r'\s*/\s*', '/', fraction_str)
-
-#     # print(f"Cleaned Fractions: {cleaned_fractions}")
-
-#     # Define the regular expression pattern to match the mixed fraction
-#     pattern = re.compile(r'\b(\d+)\s*(\d+/\d+)\b')
-#     match = pattern.search(cleaned_fractions)
-    
-#     if match:
-#         whole_number = match.group(1)
-#         fraction = match.group(2)
-#         return [whole_number, fraction]
-#     else:
-#         # If no match found, split the string based on space and return
-#         return cleaned_fractions.split()
-    
-# ####### Deprecated ####### 
-# def _sum_parsed_fractions(self, fraction_list: list, truncate = 3) -> float:
-    
-#     total = 0
-#     for i in fraction_list:
-#         total += Fraction(i)
-    
-#     return round(float(total), truncate)
-
-# regex = IngredientTools()
-
-# parenthesis = [ "(2 ounces)", 
-#                 "(about 3 cups)",
-#                 "(3)",
-#                 "(3 ounces each)", 
-#                 "(3 each)",
-#                 "(about 4 cups each)", 
-#                 "(about a couple of 3 tablespoons)", 
-#                 "(3 ounces about)"
-#                   ]
-# regex.print_matches(parenthesis[3])
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-0.0.88/ingredient_slicer/_regex_patterns.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,40 +34,35 @@
 # Generate the regular expression pattern for units in the string
 ANY_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.UNITS.values() for unit in variants_list])
 # ANY_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.UNITS.values())
 # ANY_UNIT_ALT = '|'.join('|'.join(re.escape(variant) for variant in variants) for variants in _constants.UNITS.values())
 
 # just the basic units 
 BASIC_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.BASIC_UNITS.values() for unit in variants_list])
-# BASIC_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.BASIC_UNITS.values())
 
 # just the non-basic units
 NON_BASIC_UNIT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.NON_BASIC_UNITS_SET)])
-# NON_BASIC_UNIT_ALT = '|'.join(list(_constants.NON_BASIC_UNITS_SET))
 
 # Generate the regular expression pattern for units in the string
 VOLUME_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.VOLUME_UNITS.values() for unit in variants_list])
 # VOLUME_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.VOLUME_UNITS.values())
 
 # The "sometimes might be a unit" strings as a "or" pattern
 SOMETIMES_UNIT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.SIZE_MODIFIERS_SET)])
-# SOMETIMES_UNIT_ALT = '|'.join(list(_constants.SIZE_MODIFIERS_SET))
 
 # get a pattern for the "approximate" strings (these are typically used to describe an equivelant amount of a unit)
 EQUIVALENT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.APPROXIMATE_STRINGS)])
 # EQUIVALENT_ALT = '|'.join(list(_constants.APPROXIMATE_STRINGS))
 
 # prep word alternate
 PREP_WORD_ALT = '|'.join([re.escape(prep_word) for prep_word in list(_constants.PREP_WORDS)])
 
 # sort the stopwords by their length to make sure longer stopwords get matched before shorter ones
 #  to make sure we don't match a shorter stopword that is part of a longer stopword
 STOP_WORDS_ALT = '|'.join(sorted([re.escape(stop_word) for stop_word in _constants.STOP_WORDS], key=len, reverse=True))
-# STOP_WORDS_ALT = '|'.join([re.escape(stop_word) for stop_word in list(_constants.STOP_WORDS)])
-
 
 FRACTION_WORDS_ALT = '|'.join([re.escape(fraction_word) for fraction_word in _constants.FRACTION_WORDS])
 
 # Alternations for creating patterns that match prefix number words followed by number words (e.g "twenty five", "thirty three")
 NUMBER_WORDS_ALT = '|'.join([re.escape(word) for word in _constants.NUMBER_WORDS])
 NUMBER_PREFIX_WORD_ALT = '|'.join([re.escape(word) for word in _constants.NUMBER_PREFIX_WORDS])
 
@@ -81,15 +76,14 @@
 APPROXIMATE_STRINGS_ALT = '|'.join([re.escape(approximate_string) for approximate_string in _constants.APPROXIMATE_STRINGS])
 
 # # sort the denominator words by their length to make sure longer words get matched before shorter ones
 # #  to make sure we don't match a shorter word that is part of a longer word
 # DENOMINATOR_WORDS_ALT = '|'.join(sorted([re.escape(word) for word in _constants.DENOMINATOR_WORDS], key=len, reverse=True))
 # # DENOMINATOR_WORDS_ALT = '|'.join([re.escape(word) for word in _constants.DENOMINATOR_WORDS])
 
-
 # -----------------------------------------------------------------------------
 # --------------------------- Units patterns -----------------------------
 # ---> NOTE: uses the above Alternation patterns to create the following basic regular expression patterns
 # - units in a string
 # - matching a number followed by a unit
 # - matching a unit followed by a number
 # -----------------------------------------------------------------------------
@@ -353,32 +347,29 @@
                            "NUMBER_SLASH_NUMBER", "NUMBER_SLASH_FRACTION", "FRACTION_SLASH_FRACTION", 
                            "FRACTION_SLASH_NUMBER")
 # FRACTION_TYPE_MAP = {
 #     # Starts with a decimal:
 #     "DECIMAL_SLASH_DECIMAL": re.compile(r"\d+\.\d+\s*/\s*\d+\.\d+"),
 #     "DECIMAL_SLASH_NUMBER": re.compile(r"\d+\.\d+\s*/\s*\d+"),
 #     "DECIMAL_SLASH_FRACTION": re.compile(r"\d+\.\d+\s*/\s*\d+/\d+"),
-
 #     # Starts with a whole number:
 #     "NUMBER_SLASH_DECIMAL": re.compile(r"\d+\s*/\s*\d+\.\d+"),
 #     "NUMBER_SLASH_NUMBER": re.compile(r"\d+\s*/\s*\d+"),
 #     "NUMBER_SLASH_FRACTION": re.compile(r"\d+\s*/\s*\d+/\d+"),
-
 #     # Starts with a fraction:
 #     "FRACTION_SLASH_FRACTION": re.compile(r"\d+/\d+\s*/\s*\d+/\d+"),
 #     "FRACTION_SLASH_DECIMAL": re.compile(r"\d+/\d+\s*/\s*\d+\.\d+"),
 #     "FRACTION_SLASH_NUMBER": re.compile(r"\d+/\d+\s*/\s*\d+")
 # }
 
 # FRACTION_PATTERN = re.compile(r'\d+\s*/\s*\d+') # TODO: Testing new fraction pattern, old pattern would match even if there was NOT a number in front of the forward slash...
 # FRACTION_PATTERN2 = re.compile(r'\b(\d*\.\d+|\d+)\s*/\s*(\d*\.\d+|\d+)\b')
 # NUMBER_SLASH_NUMBER = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?\s*/\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?', re.IGNORECASE)
 # NUMBER_SLASH_NUMBER = re.compile(r"\d+(?:/\d+|\.\d+)?\s*/\s*\d+(?:/\d+|\.\d+)?", re.IGNORECASE) # NOTE: NEW version (SAFE)
 
-
 # -----------------------------------------------------------------------------
 # --------------------------- Repeated strings PATTERNS -----------------------
 # Patterns to match specific cases when a known unit string is repeated in a string
 # This is typically seen in ranges where the unit appears after both quantities (e.g. 100 g - 200 g)
 # These regular expressions are used for removing the unit from the string if its repeated
 # -----------------------------------------------------------------------------
 
@@ -463,41 +454,33 @@
 PCT_REGEX_MAP = {}
 
 for pct_string in ["%", "percent", "pct"]:
     PCT_REGEX_MAP[pct_string] = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*' + pct_string + r'')
 
 # create a map containg regexs for matching a number followed by a "%", "percent", or "pct" string
 # NUMBER_WITH_DIMENSIONS_SYMBOLS_MAP = {}
-
-# NUMBER_WITH_INCH_SYMBOL.findall("1 1/2\"")
-# NUMBER_WITH_INCH_SYMBOL = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*\"')
-# NUMBER_WITH_INCH_SYMBOL = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*\”')
-# NUMBER_WITH_INCH_SYMBOL = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*\"')
-
+    
 NUMBER_WITH_INCH_SYMBOL_MAP = {}
 for inch_symbol in ["\"", "”"]:
     NUMBER_WITH_INCH_SYMBOL_MAP[inch_symbol] = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*' + inch_symbol + r'')
 
 # # -----------------------------------------------------------------------------
 # # ---------------------------- OLD IngredientTools class... ---------------------------------
 # # -----------------------------------------------------------------------------
-    
-# # -----------------------------------------------------------------------------
 # # --------------------------- Class to store all regex patterns -----------------------
 # # A class to hold all regex patterns used in the recipe parser (version 2)
 # # - Each pattern is stored as a class attribute and the class 
 # # - IngredientTools class has a single method that applies ALL of the 
 # #     regex patterns to a given string and return a dictionary of matches (for testing mainly)
 # # -----------------------------------------------------------------------------
 # # regex variables and maps to put in the class:
 # class IngredientTools:
 #     """
 #     A class to hold all regex patterns used in recipe parsing.
 #     """
-
 #     def __init__(self) -> None:
 #         # Constant data values and lookup tables
 #         self.constants = {
 
 #             # regex hashmaps
 #             "NUMBER_WORDS": _constants.NUMBER_WORDS,
 #             "NUMBER_PREFIX_WORDS": _constants.NUMBER_PREFIX_WORDS,
@@ -762,252 +745,17 @@
 #             "PCT_REGEX_MAP" : "Dictionary of regex patterns to match numbers followed by a percentage character '%', 'percentage', 'percent', or 'pct'."
 #         }
 
 #         # Retrieve description based on pattern name
 #         return descriptions.get(pattern_name, "")
     
 # ##################################################################################################################
-# ##################################################################################################################
 # ########################################## OLD SETUP CODE BELOW ##################################################
 # ##################################################################################################################
 
-# # Description: This module contains all the regex patterns used in the recipe parser. 
-# # As well as a class to hold all regex patterns used in the recipe parser (version 2)
-
-# import re
-# from typing import Dict, List, Tuple, Union
-
-# # # import constants from _constants module
-# from . import _constants 
-
-# # # import for for local development
-# # from ingredient_slicer import _constants
-
-# # -----------------------------------------------------------------------------
-# # --------------------------- Conversion patterns -----------------------------
-# # Patterns for converting: 
-# # - Fraction phrases/words to fraction strings (e.g. "one half" to "1/2")
-# # - Number words to numerical values (e.g. "one" to "1")
-# # - Unicode fractions to decimals (e.g. "½" to "0.5")
-# # -----------------------------------------------------------------------------
-
-# MULTI_FRACTION_WORDS_MAP = {}
-# for phrase, fraction in _constants.MULTI_FRACTION_WORDS.items():
-#     MULTI_FRACTION_WORDS_MAP[phrase] = [fraction, re.compile(r'\b' + phrase + r'\b', re.IGNORECASE)]
-
-# NUMBER_WORDS_MAP = {}
-# for word, value in _constants.NUMBER_WORDS.items():
-#     NUMBER_WORDS_MAP[word] = [str(value), re.compile(r'\b' + word + r'\b', re.IGNORECASE)]
-
-# # Matches unicode fractions in the string
-# UNICODE_FRACTIONS_PATTERN = re.compile( r'\b(?:' + '|'.join(re.escape(word) for word in _constants.UNICODE_FRACTIONS.keys()) + r')\b', re.IGNORECASE)
-
-# # standard_ingredient = "two third of a cups of flour, 1 half n half pint"
-
-# # # print("Parsing fraction words")
-# # for word, regex_data in MULTI_FRACTION_WORDS_MAP.items():
-# #     fraction_str, pattern = regex_data
-# #     # print(f"Word: '{word}'\n > Fraction string: '{fraction_str}'\n > Pattern: {pattern}")
-# #     if pattern.search(standard_ingredient):
-# #         print(f"Word: '{word}'\n > Fraction string: '{fraction_str}'\n > Pattern: {pattern}")
-# #         print(f"Found {word} in ingredient. Replacing with {fraction_str}")
-# #     print(f"----" * 5)
-# #     print()
-# #     # pattern = regex_data[1]
-# #     # print statement if word is found in ingredient and replaced
-# #     if pattern.search(self.standard_ingredient):
-# #         print(f"- Found {word} in ingredient. Replacing with {regex_data[0]}") if self.debug else None
-# #     self.standard_ingredient = pattern.sub(regex_data[0], self.standard_ingredient)
-
-# # -----------------------------------------------------------------------------
-# # --------------------------- Alternation patterns -----------------------------
-# # ---> NOTE: the main Alternation patterns for various units are created here and these get used in many of the other regular expression
-# # -----------------------------------------------------------------------------
-# # ---- Set up Alternation patterns from list of possible units and their variants ----
-
-# # Generate the regular expression pattern for units in the string
-# ANY_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.UNITS.values() for unit in variants_list])
-# # ANY_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.UNITS.values())
-# # ANY_UNIT_ALT = '|'.join('|'.join(re.escape(variant) for variant in variants) for variants in _constants.UNITS.values())
-
-# # just the basic units 
-# BASIC_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.BASIC_UNITS.values() for unit in variants_list])
-# # BASIC_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.BASIC_UNITS.values())
-
-# # just the non-basic units
-# NON_BASIC_UNIT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.NON_BASIC_UNITS_SET)])
-# # NON_BASIC_UNIT_ALT = '|'.join(list(_constants.NON_BASIC_UNITS_SET))
-
-# # Generate the regular expression pattern for units in the string
-# VOLUME_UNIT_ALT = '|'.join([re.escape(unit) for variants_list in _constants.VOLUME_UNITS.values() for unit in variants_list])
-# # VOLUME_UNIT_ALT = '|'.join('|'.join(variants) for variants in _constants.VOLUME_UNITS.values())
-
-# # The "sometimes might be a unit" strings as a "or" pattern
-# SOMETIMES_UNIT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.SIZE_MODIFIERS_SET)])
-# # SOMETIMES_UNIT_ALT = '|'.join(list(_constants.SIZE_MODIFIERS_SET))
-
-# # get a pattern for the "approximate" strings (these are typically used to describe an equivelant amount of a unit)
-# EQUIVALENT_ALT = '|'.join([re.escape(unit) for unit in list(_constants.APPROXIMATE_STRINGS)])
-# # EQUIVALENT_ALT = '|'.join(list(_constants.APPROXIMATE_STRINGS))
-
-# # prep word alternate
-# PREP_WORD_ALT = '|'.join([re.escape(prep_word) for prep_word in list(_constants.PREP_WORDS)])
-
-# # sort the stopwords by their length to make sure longer stopwords get matched before shorter ones
-# #  to make sure we don't match a shorter stopword that is part of a longer stopword
-# STOP_WORDS_ALT = '|'.join(sorted([re.escape(stop_word) for stop_word in _constants.STOP_WORDS], key=len, reverse=True))
-# # STOP_WORDS_ALT = '|'.join([re.escape(stop_word) for stop_word in list(_constants.STOP_WORDS)])
-
-
-# FRACTION_WORDS_ALT = '|'.join([re.escape(fraction_word) for fraction_word in _constants.FRACTION_WORDS])
-
-# # sort the denominator words by their length to make sure longer words get matched before shorter ones
-# #  to make sure we don't match a shorter word that is part of a longer word
-# DENOMINATOR_WORDS_ALT = '|'.join(sorted([re.escape(word) for word in _constants.DENOMINATOR_WORDS], key=len, reverse=True))
-# # DENOMINATOR_WORDS_ALT = '|'.join([re.escape(word) for word in _constants.DENOMINATOR_WORDS])
-
-# # Alternations for creating patterns that match prefix number words followed by number words (e.g "twenty five", "thirty three")
-# NUMBER_WORDS_ALT = '|'.join([re.escape(word) for word in _constants.NUMBER_WORDS])
-# NUMBER_PREFIX_WORD_ALT = '|'.join([re.escape(word) for word in _constants.NUMBER_PREFIX_WORDS])
-
-# # Alternations for patterns like "a pinch of" or "a handful" or "a sprinkle"
-# CASUAL_UNITS_ALT        = '|'.join([re.escape(casual_unit) for casual_unit in _constants.CASUAL_UNITS_SET])
-# CASUAL_QUANTITIES_ALT   = '|'.join([re.escape(casual_quantity) for casual_quantity in _constants.CASUAL_QUANTITIES_SET])
-
-# # alternations for remvoing useless words from the string when trying to find the food item
-# DIMENSION_UNITS_ALT     = '|'.join([re.escape(unit) for unit in _constants.DIMENSION_UNITS_SET])
-# UNIT_MODIFIERS_ALT      = '|'.join([re.escape(unit_modifier) for unit_modifier in _constants.UNIT_MODIFIERS])
-# APPROXIMATE_STRINGS_ALT = '|'.join([re.escape(approximate_string) for approximate_string in _constants.APPROXIMATE_STRINGS])
-
-
-# # -----------------------------------------------------------------------------
-# # --------------------------- Units patterns -----------------------------
-# # ---> NOTE: uses the above Alternation patterns to create the following basic regular expression patterns
-# # - units in a string
-# # - matching a number followed by a unit
-# # - matching a unit followed by a number
-# # -----------------------------------------------------------------------------
-# # ---- Use the unit varients to create the regular expression patterns ----
-
-# # create a regular expression pattern to match the units in a string
-# UNITS_PATTERN = re.compile(r'\b(?:' + ANY_UNIT_ALT + r')\b', re.IGNORECASE)
-# # UNITS_PATTERN = re.compile(r'\b(?:' + '|'.join('|'.join(variants) for variants in UNITS.values()) + r')\b', re.IGNORECASE)
-
-# # match just the basic units
-# BASIC_UNITS_PATTERN = re.compile(r'\b(?:' + BASIC_UNIT_ALT + r')\b', re.IGNORECASE)
-
-# # match just the non-basic units
-# NON_BASIC_UNITS_PATTERN = re.compile(r'\b(?:' + NON_BASIC_UNIT_ALT + r')\b', re.IGNORECASE)
-
-# # match the "sometimes might be a unit" strings
-# SIZE_MODIFIERS_PATTERN = re.compile(r'\b(?:' + SOMETIMES_UNIT_ALT + r')\b', re.IGNORECASE)
-# # SIZE_MODIFIERS_PATTERN = re.compile(r'\b(?:' + '|'.join(SIZE_MODIFIERS_SET) + r')\b', re.IGNORECASE)
-
-# # create a regular expression pattern to match specifically volume units in a string
-# VOLUME_UNITS_PATTERN = re.compile(r'\b(?:' + VOLUME_UNIT_ALT + r')\b', re.IGNORECASE)
-
-# # generic prep words pattern for matching prep words in a string
-# PREP_WORDS_PATTERN = re.compile(r'\b(?:' + PREP_WORD_ALT + r')\b', re.IGNORECASE)
-
-# # general stop words pattern for matching stop words in a string
-# STOP_WORDS_PATTERN = re.compile(r'\b(?:' + STOP_WORDS_ALT + r')\b', re.IGNORECASE)
-
-# # match word versions of fractions in a string (e.g. "half", "thirds")
-# FRACTION_WORDS_PATTERN = re.compile(r'\b(?:' + FRACTION_WORDS_ALT + r')\b', re.IGNORECASE)
-
-# # patterns for things like "a pinch of" or "a handful" or "a sprinkle"
-# CASUAL_UNITS_PATTERN       = re.compile(r'\b(?:' + CASUAL_UNITS_ALT + r')\b', re.IGNORECASE) # e.g. "bunch", "sprig", "stalk", "stick", "piece", "slice", "strip", "strip", "segment", "wedge", "chunk", "hunk", "slab", "sliver", "shred", "shard", "scrap", "scrape", "scraping", "scrapings
-# CASUAL_QUANTITIES_PATTERN   = re.compile(r'\b(?:' + CASUAL_QUANTITIES_ALT + r')\b', re.IGNORECASE) # e.g. "a few", "a couple", "a handful", "a pinch", "a sprinkle", "a dash", "a smidgen", "a touch", "a bit"
-
-# # Miscellaneous patterns used for trimmin the string down to get the food item 
-# DIMENSION_UNITS_PATTERN     = re.compile(r'\b(?:' + DIMENSION_UNITS_ALT + r')\b', re.IGNORECASE) # e.g. "inch", "inches", "cm", "mm", "millimeter", "millimeters", "centimeter", "centimeters"
-# UNIT_MODIFIERS_PATTERN      = re.compile(r'\b(?:' + UNIT_MODIFIERS_ALT + r')\b', re.IGNORECASE) # e.g. "large", "small", "medium
-# APPROXIMATE_STRINGS_PATTERN = re.compile(r'\b(?:' + APPROXIMATE_STRINGS_ALT + r')\b', re.IGNORECASE) # e.g. "about", "approximately", "around", "roughly", "nearly", "almost
-
-
-# # -----------------------------------------------------------------------------
-# # --------------------------- Prefix number words with number words patterns -----------------------------
-# # Patterns for matching:
-# # - prefix number words followed by number words (e.g "twenty five", "thirty three")
-# # -----------------------------------------------------------------------------
-
-# # regular expression pattern to match prefix number words followed by number words
-# PREFIXED_NUMBER_WORDS = re.compile(r'\b(?:' + NUMBER_PREFIX_WORD_ALT + r')(?:\s*[-\s]*\s*)(?:' + NUMBER_WORDS_ALT + r')\b', re.IGNORECASE)
-# # PREFIXED_NUMBER_WORDS = re.compile(r'\b(?:' + NUMBER_PREFIX_WORD_ALT + r')(?:\s*|\s*-*\s*)(?:' + NUMBER_WORDS_ALT + r')\b', re.IGNORECASE)
-
-# # PREFIXED_NUMBER_WORDS_GROUPS = re.compile(r'\b(' + NUMBER_PREFIX_WORD_ALT + r')(?:\s*[-\s]*\s*)(' + NUMBER_WORDS_ALT + r')\b', re.IGNORECASE) # OG
-# PREFIXED_NUMBER_WORDS_GROUPS = re.compile(r'\b(' + NUMBER_PREFIX_WORD_ALT + r')(?:[-\s]*)(' + NUMBER_WORDS_ALT + r')\b', re.IGNORECASE) # NEW
-# # PREFIXED_NUMBER_WORDS_GROUPS = re.compile(r'\b(' + NUMBER_PREFIX_WORD_ALT + r')[-\s](' + NUMBER_WORDS_ALT + r')\b', re.IGNORECASE)
-
-# PREFIXED_NUMBER_WORDS_MAP = {}
-# for prefix_word, prefix_number in _constants.NUMBER_PREFIX_WORDS.items():
-#     for number_word, number_value in _constants.NUMBER_WORDS.items():
-#         PREFIXED_NUMBER_WORDS_MAP[prefix_word + " " + number_word] = [str(prefix_number + number_value), re.compile(r'\b' + prefix_word + r'(?:[-\s]*)' + number_word + r'\b', re.IGNORECASE)]
-
-# # ----------------------------------------------------------------------------------------------------------------------
-# # --------------------------- Unit/Number or Number/Unit patterns -----------------------------
-# # Patterns for matching:
-# # - a number followed by a unit
-# # - a unit followed by a number
-# # - a number followed by a unit followed by any text (full unit and abbreviation)
-# # - a unit followed by a number followed by any text (full unit and abbreviation)
-# # - a number/decimal/fraction followed by a space and then another number/decimal/fraction
-# # - a number/decimal/fraction followed by a space and then another number/decimal/fraction followed by a unit
-# # -----------------------------------------------------------------------------
-# # ----------------------------------------------------------------------------------------------------------------------
-
-# # Construct the regular expression pattern that matches the number (including fractions and decimals)
-# # followed by 0+ spaces and then a unit in UNITS dictionary
-# ANY_NUMBER_THEN_UNIT = re.compile(r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*(?:' + ANY_UNIT_ALT + r')\b')
-# # ANY_NUMBER_THEN_UNIT = r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*(?:' + ANY_UNIT_ALT + r')\b'
-
-# # Construct the regular expression pattern that matches the number (including fractions and decimals)
-# # followed by any text and then a unit in UNITS dictionary
-# ANY_NUMBER_THEN_ANYTHING_THEN_UNIT = re.compile(r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*.*?\s*(?:' + ANY_UNIT_ALT + r')\b')
-
-# # same as above but with 2 capture groups (number and unit)
-# ANY_NUMBER_THEN_ANYTHING_THEN_UNIT_GROUPS  = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s+(\S*\b(?:' + ANY_UNIT_ALT + r'))\b')
-# # ANY_NUMBER_THEN_ANYTHING_THEN_UNIT_GROUPS2 = re.compile(r'\b(\d+)\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-
-# r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(can|cup|cups|cabin)\b'
-# # same as above but with 2 capture groups (number and unit, either basic, non-basic, or any unit)
-# QUANTITY_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-# QUANTITY_BASIC_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + BASIC_UNIT_ALT + r')\b')
-# QUANTITY_NON_BASIC_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + NON_BASIC_UNIT_ALT + r')\b')
-# QUANTITY_SOMETIMES_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + SOMETIMES_UNIT_ALT + r')\b')
-# QUANTITY_DIMENSION_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + DIMENSION_UNITS_ALT + r')\b')
-
-# QUANTITY_ANYTHING_UNIT_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-
-# # restrictive quantity unit group matcher, matches a quantity number followed by 0+ whitespaces/0+ hyphens and then a unit in ANY_UNIT_ALT
-# # (i.e. "1 cup", "1-1/2 cup", "12 -- cup")
-# QUANTITY_UNIT_ONLY_GROUPS = re.compile(r'\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*[-\s]*\b(' + ANY_UNIT_ALT + r')\b')
-
-# # Pattern for finding quantity unit patterns that are preceeded by an "equivalent" string 
-# # (i.e. "about 1/2 cup", "about 3 tablespoons", "approximately 1/2 cup", "approximately 3 tablespoons")
-# EQUIV_QUANTITY_UNIT_GROUPS = re.compile(r'\b(' + EQUIVALENT_ALT + r')\b\s*.*?\s*\b((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-# # EQUIV_QUANTITY_UNIT_GROUPS = re.compile(r'\b(' + EQUIVALENT_ALT + r')\s+((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-# # EQUIVALENT_QUANTITY_UNIT_GROUPS = re.compile(r'\b(' + EQUIVALENT_ALT + r')\s+((?:\d*\.\d+|\d+\s*/\s*\d+|\d+))\s*.*?\s*\b(' + ANY_UNIT_ALT + r')\b')
-
-# # a number/decimal/fraction followed by 1+ spaces to another number/decimal/fraction followed by a 0+ spaces then a VOLUME unit
-# # (e.g. 1/2 cup, 1 1/2 cups, 1 1/2 tablespoon)
-# SPACED_NUMS_THEN_VOLUME_UNITS = re.compile(r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)+\s*(?:\d+/\d+|\d+\.\d+)\s*(?:' + VOLUME_UNIT_ALT + r')\b')
-
-# # Construct the regular expression pattern that matches the number (including fractions and decimals)
-# # followed by 0+ spaces and then a unit in UNITS dictionary (EXPIREMENTAL, probably throw away)
-# ANY_NUMBER_THEN_UNIT_CAPTURE = re.compile(r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*(.*?)*(?:' + ANY_UNIT_ALT + r')\b')
-
-# # Construct the regular expression pattern that matches the unit followed by 0+ spaces
-# # and then a number (including fractions and decimals)
-# UNIT_THEN_ANY_NUMBER = re.compile(r'\b(?:' + ANY_UNIT_ALT + r')\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\b')
-# # UNIT_THEN_ANY_NUMBER = r'\b(?:' + ANY_UNIT_ALT + r')\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\b'
-
-# # Regex to match number (QUANTITY) then unit abbreviation (single string as unit)
-# NUMBER_THEN_UNIT_ABBR = re.compile(r"(\d)\-?([a-zA-Z])") # 3g = 3 g
-
 # # Regex to match number (QUANTITY) then unit word (full word string as unit)
 # NUMBER_THEN_UNIT_WORD = re.compile(r"(\d+)\-?([a-zA-Z]+)") #  "3tbsp vegetable oil" = 3 tbsp
 
 # # ----------------------------------------------------------------------------------------------------------------------
 # # --------------------------- Generic number patterns and numbers w/ specific separators -----------------------------
 # # Patterns for matching:
 # # - a number/decimal/fraction followed by a space and then another number/decimal/fraction
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer/_utils.py` & `ingredient_slicer-0.0.88/ingredient_slicer/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,37 +157,25 @@
         Args:
             fraction_str (str): The string representation of the fraction. Must only contain digits, a forward slash, and possible whitespace. 
                                     Numbers must be separated by a forward slash. If a whole number string or a decimal string is passed, it will be returned as a string, 
                                     and converted to a whole number if values after the decimal point are only zeros (i.e. 1.0 -> 1, 2.0 -> 2, 3.00 -> 3).
         Returns:
             str: The decimal value of the fraction as a string. 
         """
-        # FRACTION_PATTERN2 = re.compile(r'\d+(?:\.\d+|/\d+)')
-
-        # fraction_str = "4/0.48"
-        # fraction_str = "4/0.48."
-        # fraction_str = ".3/4"
-        # FRACTION_PATTERN2.findall(fraction_str)
-        # 4/0.48
         
         if not isinstance(fraction_str, str):
             raise ValueError("Invalid input. Fraction string must be a string.")
 
         # Split the fraction string into its numerator and denominator
         split_fraction = [i.strip() for i in fraction_str.split("/")]
         # print(f"Split Fraction: {split_fraction}") if self.debug else None
 
         # If the fraction is a whole number, return the number
         if len(split_fraction) == 1:
-            # print(f"---> Only one part: {split_fraction[0]}")
-
             converted_number = _make_int_or_float_str(split_fraction[0])
-
-            # print(f"---> OLD Output: {round(float(split_fraction[0]), 3)}")
-            # print(f"---> NEW Output: {converted_number}")
             return converted_number
         
         # remove trailing period if it exists
         if split_fraction[1][-1] == ".":
             split_fraction[1] = split_fraction[1][:-1]
 
         # after returning cases of just a whole number or decimal number and returning that, 
@@ -286,23 +274,14 @@
 
 #         fraction_decimal = _fraction_str_to_decimal(match)
 #         # print(f"Fraction Decimal: {fraction_decimal}") if self.debug else None
 #         ingredient = ingredient.replace(match, str(fraction_decimal))
 
 #     return ingredient
 
-# TODO: USE these as a basis for tests
-# ingredient = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon"
-# _convert_fractions_to_decimals(ingredient)
-# _convert_fractions_to_decimals2(ingredient)
-
-# ingredient = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon, 2.0/4"
-# _convert_fractions_to_decimals(ingredient)
-# _convert_fractions_to_decimals2(ingredient)
-
 # -----------------------------------------------------------------------------------------------------------------------
 # ---- Force whitespaces between an number followed by a character or vice versa (i.e. "1cup" -> "1 cup") ----
 # -----------------------------------------------------------------------------------------------------------------------
 
 def _force_ws_between_numbers_and_chars(ingredient: str) -> str:
     
     """Forces spaces between numbers and units and between units and numbers.
@@ -472,18 +451,16 @@
         Returns:
             str: The updated ingredient string with "a" or "an" replaced with "1" if no other quantites are found.
         """
 
         if not isinstance(ingredient, str):
             raise ValueError("Invalid input. Ingredient must be a string.")
 
-        # regex_patterns = _regex_patterns.IngredientTools()
-
         # lowercase and split the ingredient string
-        ingredient = ingredient.lower()
+        ingredient       = ingredient.lower()
         split_ingredient = ingredient.split()
 
         quantity_matches = re.findall(_regex_patterns.ALL_NUMBERS, ingredient)
 
         # if no quantities are found in the ingredient string, 
         # look for and replace the first "a" or "an" with "1"
         if not quantity_matches:
@@ -662,44 +639,23 @@
 
 #     assert parsed['secondary_quantity'] == None  # TODO: maybe this case should get a quantity of 1, but for now it's None
 #     assert parsed['secondary_unit'] == "breast"
 #     assert parsed['standardized_secondary_unit'] == "breast"
 
 #     assert parsed['is_required'] == True
 
-
-# ingredient = '1 cup of chopped chicken breast (about 12 ounces)'
-# EQUIV_QUANTITY_UNIT_GROUPS
-# QUANTITY_UNIT_GROUPS
-# regex_patterns = _regex_patterns.IngredientTools()
-
-# # ingredient = "1 cup of chopped chicken breast (about 12 ounces)"
-# ingredient = '1 cup of chopped chicken breast (about 12 tender and juicy ounces)'
-# parenthesis_content = ['(about 12 tender and juicy ounces)']
-# # parenthesis_content = ['(about tender and juicy ounces)']
-# parenthesis = parenthesis_content[0]
-
-# _regex_patterns.EQUIV_QUANTITY_UNIT_GROUPS.findall(parenthesis)
-
 def _extract_quantities_only(input_string: str) -> list:
 
     """From a string get all quantities if they exist WITHOUT units
     Useful for just getting quantities if there are no units associated with them (e.g. "chicken breast (5)")
     Args:
         input_string (str): The string to parse
     Returns:
         list: A list of quantities
     """
-
-    # input_string = parenthesis
-    # input_string = '(about 12 tender and juicy ounces or about 14 grams)'
-    # input_string = '(about 12 tender and juicy ounces)'
-    # input_string = '(14 cups)'
-    # input_string = '(juicy about 14 ,  and 456)'
-
     if not isinstance(input_string, str):
         raise ValueError("Invalid input. Input must be a string.")
 
     # regex_patterns = _regex_patterns.IngredientTools()
 
     # first check for units
     unit_matches = _regex_patterns.UNITS_PATTERN.findall(input_string)
@@ -726,20 +682,15 @@
     """From a string get all sets of quantity/units
     Useful for getting quantity/units pairings from a string (e.g. "1 cup of chopped chicken breast")
     Args:
         input_string (str): The string to parse
     Returns:
         list: A list of tuples containing the quantity and unit
     """
-
-    # input_string = parenthesis
-    # input_string = '(about 12 tender and juicy ounces or about 14 grams)'
-    # input_string = '(about 12 tender and juicy ounces)'
-    # input_string = '(juicy about or 14)'
-
+    
     if not isinstance(input_string, str):
         raise ValueError("Invalid input. Input must be a string.")
 
     # regex_patterns = _regex_patterns.IngredientTools()
 
     # regex_patterns.QUANTITY_UNIT_GROUPS.findall(input_string)
     quantity_matches = _regex_patterns.ALL_NUMBERS.finditer(input_string)
@@ -2280,36 +2231,7 @@
 #             # if replacement_function:
 #             #     print(f"Replacement Function given")
 #             #     updated_range = replacement_function(updated_range)
 #             ingredient = ingredient.replace(original_range, updated_range)
 #             # print("\n") if self.debug else None
 
 #         return ingredient
-# def _update_ranges(self, ingredient: str, pattern: re.Pattern, replacement_function=None) -> str:
-#     """Update the ranges in the ingredient string with the updated ranges
-#     Args:
-#         ingredient (str): The ingredient string to update
-#         pattern (re.Pattern): The pattern to use to find the ranges
-#         replacement_function (function, optional): A function to use to replace the matched ranges. Defaults to None.
-#     Returns:
-#         str: The updated ingredient string
-#     """
-    
-#     matches = pattern.findall(ingredient)
-#     # matched_ranges = [match.split("-") for match in matches]
-
-#     if replacement_function:
-#         matched_ranges = [replacement_function(match).split("-") for match in matches]
-#     else:
-#         matched_ranges = [match.split("-") for match in matches]
-
-#     updated_ranges = [" - ".join([str(_utils._fraction_str_to_decimal(i)) for i in match if i]) for match in matched_ranges]
-#     # updated_ranges = [" - ".join([str(int(i)) for i in match if i]) for match in matched_ranges]
-    
-#     # Create a dictionary to map the matched ranges to the updated ranges
-#     ranges_map = dict(zip(matches, updated_ranges))
-
-#     # Replace the ranges in the original string with the updated ranges
-#     for original_range, updated_range in ranges_map.items():
-#         ingredient = ingredient.replace(original_range, updated_range)
-
-#     return ingredient
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-0.0.88/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.87
+Version: 0.0.88
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-0.0.87/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-0.0.88/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/pyproject.toml` & `ingredient_slicer-0.0.88/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "0.0.87"
+version = "0.0.88"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-0.0.87/tests/test_avg_ranges.py` & `ingredient_slicer-0.0.88/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_casual_ingredients.py` & `ingredient_slicer-0.0.88/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-0.0.88/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-0.0.88/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-0.0.88/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_extract_dimensions.py` & `ingredient_slicer-0.0.88/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_extract_quantities_utils.py` & `ingredient_slicer-0.0.88/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_find_and_remove.py` & `ingredient_slicer-0.0.88/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-0.0.88/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-0.0.88/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_get_gram_weight.py` & `ingredient_slicer-0.0.88/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_ingredient_slicer.py` & `ingredient_slicer-0.0.88/tests/test_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pytest
 
 import re
 
 from ingredient_slicer import IngredientSlicer
 
 # -------------------------------------------------------------------------------
+
 # -------------------------------------------------------------------------------
 # ---- Simple standard form ingredients tests ----
 # Standard form: "1 cup of sugar" (quantity, unit, ingredient)
 # -------------------------------------------------------------------------------
 
 def test_standard_formatted_ingredients():
```

### Comparing `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-0.0.88/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-0.0.88/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_make_int_or_float_str.py` & `ingredient_slicer-0.0.88/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-0.0.88/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_merge_numbers.py` & `ingredient_slicer-0.0.88/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_number_ranges.py` & `ingredient_slicer-0.0.88/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-0.0.88/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-0.0.88/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_parenthesis.py` & `ingredient_slicer-0.0.88/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_parenthesis_utils.py` & `ingredient_slicer-0.0.88/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_percentages.py` & `ingredient_slicer-0.0.88/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-0.0.88/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_prep_words.py` & `ingredient_slicer-0.0.88/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_quantity_range_regex.py` & `ingredient_slicer-0.0.88/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_quantity_units_regex.py` & `ingredient_slicer-0.0.88/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-0.0.88/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_remove_x_separators.py` & `ingredient_slicer-0.0.88/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-0.0.88/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_separate_dimensions.py` & `ingredient_slicer-0.0.88/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_size_modifiers.py` & `ingredient_slicer-0.0.88/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_spaced_numbers.py` & `ingredient_slicer-0.0.88/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_unit_regex.py` & `ingredient_slicer-0.0.88/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_wild_ingredients.py` & `ingredient_slicer-0.0.88/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_word_fractions.py` & `ingredient_slicer-0.0.88/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_word_numbers.py` & `ingredient_slicer-0.0.88/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.87/tests/test_x_after_number_regex.py` & `ingredient_slicer-0.0.88/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

