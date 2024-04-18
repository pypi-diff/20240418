# Comparing `tmp/chemistry_tools-1.0.0b2.tar.gz` & `tmp/chemistry_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_tools-1.0.0b2.tar", last modified: Thu Jul 13 20:50:11 2023, max compression
+gzip compressed data, was "chemistry_tools-1.0.1.tar", last modified: Thu Apr 18 14:19:19 2024, max compression
```

## Comparing `chemistry_tools-1.0.0b2.tar` & `chemistry_tools-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-07-13 20:50:11.320987 chemistry_tools-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-13 20:50:11.324987 chemistry_tools-1.0.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9971 2023-07-13 20:50:11.328987 chemistry_tools-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-13 20:50:11.312987 chemistry_tools-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6895 2023-07-13 20:50:11.324987 chemistry_tools-1.0.0b2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/_memoized_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/toxnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/cas.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/spectrum_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8040 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/units.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/_memoized_property.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/names.py
--rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/property_format.py
--rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/lanthanides.py
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_isotope_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/chalcogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/pnictogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/alkaline_earth_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/noble_gases.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/alkali_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/transition_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_elements.py
--rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/halogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/triels.py
--rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/tetrels.py
--rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/actinides.py
--rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/html.py
--rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/species.py
--rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/iso_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)     6979 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/latex.py
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/composition.py
--rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/_parser_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/unicode.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/full_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/description.py
--rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/bond.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14771 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     5676 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/atom.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/pug_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/synonyms.py
--rw-r--r--   0 runner    (1001) docker     (122)    19312 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 14:19:19.528224 chemistry_tools-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-18 14:19:19.532224 chemistry_tools-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-18 14:19:19.536224 chemistry_tools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-18 14:19:19.532224 chemistry_tools-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 14:19:19.532224 chemistry_tools-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/property_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-18 14:18:53.992365 chemistry_tools-1.0.1/chemistry_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 14:18:53.992365 chemistry_tools-1.0.1/chemistry_tools/_memoized_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/toxnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17944 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/spectrum_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 14:18:53.992365 chemistry_tools-1.0.1/chemistry_tools/_memoized_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/chalcogens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/alkaline_earth_metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/triels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/halogens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64225 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/transition_metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/actinides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/_isotope_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/noble_gases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/pnictogens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14069 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/alkali_metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/tetrels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33686 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/lanthanides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19571 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/elements/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/_parser_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27405 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/iso_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/formulae/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19312 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9048 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/pug_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/full_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-18 14:18:53.996365 chemistry_tools-1.0.1/chemistry_tools/pubchem/enums.py
```

### Comparing `chemistry_tools-1.0.0b2/pyproject.toml` & `chemistry_tools-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "chemistry_tools"
-version = "1.0.0b2"
+version = "1.0.1"
 description = "Python tools for analysis of chemical compounds."
 readme = "README.rst"
 keywords = [ "chemistry", "utility",]
 dynamic = []
 dependencies = [
     "apeye>=0.9.1",
     "cachecontrol>=0.13.1",
@@ -29,34 +29,34 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Database :: Front-Ends",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/domdfcoding/chemistry_tools"
 "Issue Tracker" = "https://github.com/domdfcoding/chemistry_tools/issues"
 "Source Code" = "https://github.com/domdfcoding/chemistry_tools"
 Documentation = "https://chemistry-tools.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
@@ -87,15 +87,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Database :: Front-Ends",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "LGPL-3.0-or-later"
 additional-files = [ "recursive-include chemistry_tools requirements.txt",]
 
 [tool.sphinx-pyproject]
 github_username = "domdfcoding"
@@ -114,29 +114,27 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "enum_tools.autoenum",
     "_internal_extension",
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_toolbox.latex.succinct_seealso",
     "sphinx_toolbox_experimental.missing_xref",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -188,30 +186,30 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.dep_checker]
 allowed_unused = [ "cachecontrol", "lockfile", "filelock",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `chemistry_tools-1.0.0b2/PKG-INFO` & `chemistry_tools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: chemistry-tools
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: Python tools for analysis of chemical compounds.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: LGPL-3.0-or-later
 Keywords: chemistry,utility
 Home-page: https://github.com/domdfcoding/chemistry_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/chemistry_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/chemistry_tools
@@ -20,14 +20,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
@@ -167,23 +168,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.1
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/chemistry_tools
 	:target: https://pypi.org/project/chemistry_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `chemistry_tools-1.0.0b2/LICENSE` & `chemistry_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/README.rst` & `chemistry_tools-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.1
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/chemistry_tools
 	:target: https://pypi.org/project/chemistry_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/toxnet.py` & `chemistry_tools-1.0.1/chemistry_tools/toxnet.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/cas.py` & `chemistry_tools-1.0.1/chemistry_tools/cas.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/spectrum_similarity.py` & `chemistry_tools-1.0.1/chemistry_tools/spectrum_similarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,18 @@
 		Returns the similarity score.
 		"""
 
 		# Unimplemented R code
 		# alignment <- alignment[alignment[,1] >= x.threshold, ]
 
 		similarity_score = self._calculate_score(self.alignment)
-		reverse_similarity_score = self._calculate_score(self.reverse_alignment)
+		if self.reverse_alignment.empty:
+			reverse_similarity_score = 0.0
+		else:
+			reverse_similarity_score = self._calculate_score(self.reverse_alignment)
 
 		return similarity_score, reverse_similarity_score
 
 	def plot(
 			self,
 			top_label: Optional[str] = None,
 			bottom_label: Optional[str] = None,
```

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/units.py` & `chemistry_tools-1.0.1/chemistry_tools/units.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/cache.py` & `chemistry_tools-1.0.1/chemistry_tools/cache.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/names.py` & `chemistry_tools-1.0.1/chemistry_tools/names.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/constants.py` & `chemistry_tools-1.0.1/chemistry_tools/constants.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/__init__.py` & `chemistry_tools-1.0.1/chemistry_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/property_format.py` & `chemistry_tools-1.0.1/chemistry_tools/property_format.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/lanthanides.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/lanthanides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/_table.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/_table.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/_isotope_data.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/_isotope_data.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/chalcogens.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/chalcogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/pnictogens.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/pnictogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/classes.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/classes.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/alkaline_earth_metals.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/alkaline_earth_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/noble_gases.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/noble_gases.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/__init__.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/alkali_metals.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/alkali_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/transition_metals.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/transition_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/_elements.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/_elements.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/halogens.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/halogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/triels.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/triels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/tetrels.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/tetrels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/elements/actinides.py` & `chemistry_tools-1.0.1/chemistry_tools/elements/actinides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/utils.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
 		>>> for i in hill_order("H", "C[12]", "O"): print(i, end='')
 		CHO
 	"""
 
 	symbols_list: List[str] = list(set(symbols))
 
 	carbon_isotopes = list(filter(_hill_carbon_re.findall, symbols_list))
-	print(carbon_isotopes)
+	# print(carbon_isotopes)
 
 	if carbon_isotopes:
 		for isotope in sorted(carbon_isotopes):
 			symbols_list.remove(isotope)
 			yield isotope
 
 		hydrogen_isotopes = list(filter(_hill_hydrogen_re.findall, symbols_list))
```

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/html.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/html.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/species.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/species.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/dataarray.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/dataarray.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/parser.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/parser.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/iso_dist.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/iso_dist.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/compound.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/compound.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/__init__.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/latex.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/latex.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/composition.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/composition.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/_parser_core.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/_parser_core.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/formula.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/formula.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/formulae/unicode.py` & `chemistry_tools-1.0.1/chemistry_tools/formulae/unicode.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/lookup.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/lookup.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/full_record.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/full_record.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/utils.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/description.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/description.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/errors.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/errors.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/bond.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/bond.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/enums.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.pyi` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/enums.pyi`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/compound.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/compound.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/atom.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/atom.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/images.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 
 # stdlib
 from io import BytesIO
 from typing import Sequence, Union
 
 # 3rd party
-from PIL import Image  # type: ignore[import]  # nodep
+from PIL import Image  # nodep
 
 # this package
 from .enums import PubChemNamespace
 from .pug_rest import do_rest_get
 
 __all__ = ["get_structure_image"]
```

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/__init__.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/pug_rest.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/pug_rest.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/synonyms.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/synonyms.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/properties.py` & `chemistry_tools-1.0.1/chemistry_tools/pubchem/properties.py`

 * *Files identical despite different names*

