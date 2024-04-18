# Comparing `tmp/schwifty-2024.1.1.post0.tar.gz` & `tmp/schwifty-2024.4.0.tar.gz`

## Comparing `schwifty-2024.1.1.post0.tar` & `schwifty-2024.4.0.tar`

### file list

```diff
@@ -1,128 +1,129 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.envrc
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.readthedocs.yml
--rw-r--r--   0        0        0    18677 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/CHANGELOG.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/Makefile
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/devbox.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/devbox.lock
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/Makefile
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/requirements.txt
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/changelog.rst
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/conf.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/examples.rst
--rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/ilikewhatugot.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/index.rst
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/__init__.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bban.py
--rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bic.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/common.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/domain.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/exceptions.py
--rw-r--r--   0        0        0    12304 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/iban.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/py.typed
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/registry.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/README.md
--rw-r--r--   0        0        0   191918 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_at.json
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ba.json
--rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_be.json
--rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ch.json
--rw-r--r--   0        0        0    11990 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_cz.json
--rw-r--r--   0        0        0  1063746 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_de.json
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ee.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_es.json
--rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_fi.json
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ge.json
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_hr.json
--rw-r--r--   0        0        0    31241 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_hu.json
--rw-r--r--   0        0        0    62122 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_it.json
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_kz.json
--rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lt.json
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lu.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lv.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_md.json
--rw-r--r--   0        0        0    14630 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_nl.json
--rw-r--r--   0        0        0   407141 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_no.json
--rw-r--r--   0        0        0   767956 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_pl.json
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ro.json
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_rs.json
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_se.json
--rw-r--r--   0        0        0   145316 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_si.json
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_sk.json
--rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ua.json
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ad.json
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ae.json
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_bg.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_cr.json
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_cy.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_dk.json
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_es.json
--rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_fr.json
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_gb.json
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_gr.json
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ie.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_il.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_is.json
--rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_it.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_mc.json
--rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_pt.json
--rw-r--r--   0        0        0    27620 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_sa.json
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/bank_registry/manual_tr.json
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/albania.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/belgium.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/czech_republic.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/estonia.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/finland.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/france.py
--rw-r--r--   0        0        0    15548 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/germany.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/iceland.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/iso7064_mod97_10.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/iso7064_mod97_10_variant.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/italy.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/netherlands.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/norway.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/poland.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/registry.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/checksum/spain.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/iban_registry/README.md
--rw-r--r--   0        0        0    33005 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/iban_registry/generated.json
--rw-r--r--   0        0        0    16902 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/schwifty/iban_registry/overwrite.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/Dockerfile_se
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_at.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_be.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_ch.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_cz.py
--rwxr-xr-x   0        0        0     2004 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_de.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_es.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_fi.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_hr.py
--rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_hu.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_it.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_lt.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_lv.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_nl.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_no.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_pl.py
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_ro.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_se.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_si.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_sk.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_bank_registry_ua.py
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/get_iban_registry.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/requirements.txt
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/scripts/update-all.sh
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/tests/test_bic.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/tests/test_checksum.py
--rw-r--r--   0        0        0    14787 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/tests/test_iban.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/tests/test_registry.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/LICENSE
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/README.rst
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/hatch.toml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/pyproject.toml
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 schwifty-2024.1.1.post0/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.envrc
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0    19801 2020-02-02 00:00:00.000000 schwifty-2024.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.4.0/Makefile
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.4.0/devbox.json
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.4.0/devbox.lock
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/Makefile
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/examples.rst
+-rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/ilikewhatugot.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.4.0/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/__init__.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bban.py
+-rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bic.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/common.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/domain.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/exceptions.py
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/iban.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/py.typed
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/registry.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/README.md
+-rw-r--r--   0        0        0   191918 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_at.json
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ba.json
+-rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_be.json
+-rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ch.json
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_cz.json
+-rw-r--r--   0        0        0  1063746 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_de.json
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ee.json
+-rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_es.json
+-rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_fi.json
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ge.json
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_hr.json
+-rw-r--r--   0        0        0    31241 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_hu.json
+-rw-r--r--   0        0        0    62122 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_it.json
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_kz.json
+-rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_lt.json
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_lu.json
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_lv.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_md.json
+-rw-r--r--   0        0        0    14630 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_nl.json
+-rw-r--r--   0        0        0   407141 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_no.json
+-rw-r--r--   0        0        0   767956 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_pl.json
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ro.json
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_rs.json
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_se.json
+-rw-r--r--   0        0        0   145316 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_si.json
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_sk.json
+-rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/generated_ua.json
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_ad.json
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_ae.json
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_bg.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_cr.json
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_cy.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_dk.json
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_es.json
+-rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_fr.json
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_gb.json
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_gr.json
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_ie.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_il.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_is.json
+-rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_it.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_mc.json
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_me.json
+-rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_pt.json
+-rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_sa.json
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/bank_registry/manual_tr.json
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/albania.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/belgium.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/czech_republic.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/estonia.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/finland.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/france.py
+-rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/germany.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/iceland.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/iso7064_mod97_10.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/iso7064_mod97_10_variant.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/italy.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/netherlands.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/norway.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/poland.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/registry.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/checksum/spain.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/iban_registry/README.md
+-rw-r--r--   0        0        0    33005 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/iban_registry/generated.json
+-rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.4.0/schwifty/iban_registry/overwrite.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/Dockerfile_se
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_at.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_be.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_ch.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_cz.py
+-rwxr-xr-x   0        0        0     2004 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_de.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_es.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_fi.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_hr.py
+-rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_hu.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_it.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_lt.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_lv.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_nl.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_no.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_pl.py
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_ro.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_se.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_si.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_sk.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_bank_registry_ua.py
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/get_iban_registry.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/requirements.txt
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.4.0/scripts/update-all.sh
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 schwifty-2024.4.0/tests/test_bic.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.4.0/tests/test_checksum.py
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 schwifty-2024.4.0/tests/test_iban.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.4.0/tests/test_registry.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.4.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.4.0/README.rst
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.4.0/hatch.toml
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 schwifty-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 schwifty-2024.4.0/PKG-INFO
```

### Comparing `schwifty-2024.1.1.post0/CHANGELOG.rst` & `schwifty-2024.4.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `CalVer <http://www.calver.org/>`_ with the scheme ``YY.0M.Micro``.
 
+`2024.04.0`_ - 2024/04/18
+-------------------------
+Added
+~~~~~
+* Added Revolut Bank for Spain `@brunovilla <https://github.com/brunovila>`_
+* Added support for Python 3.12
+* Added manually curated bank registry for Montenegro `@Djuka <https://github.com/Djuka>`_
+
+Changed
+~~~~~~~
+* The bank registry is now internally validated, so that all domestic bank codes actaully match the
+  specification of the corresponding BBAN structure. As a result some entries had to be removed,
+  because they did contain invalid bank codes.
+* The Danish national checksum algorithm is considered opaque and the checksum digit is assumed to
+  be part of the account number (which is now always 10 digits long).
+
+Fixed
+~~~~~
+* The Czech bank registry was stored in latin-1 encoding while being read as UTF-8. This resulted
+  in invalid bank names `@Natim <https://github.com/Natim>`_ and
+  `@Cogax <https://github.com/Cogax>`_.
+* The Norwegian national checksum algorithm was rendering wrong results in some edge-cases
+  `@Natim <https://github.com/Natim>`_
+
+
+
 `2024.01.1`_ - 2024/01/05
 -------------------------
 Added
 ~~~~~
 
 * Support aspirational countries:
 
@@ -19,17 +45,17 @@
   * Burundi
   * Cabo Verde
   * Cameroon
   * Central African Republic
   * Chad
   * Comoros
   * Congo
-  * Cote d'Ivoire
+  * Côte d'Ivoire
   * Djibouti
-  * Equatorial Gunea
+  * Equatorial Guinea
   * Gabon,
   * Guinea-Bissau
   * Honduras
   * Iran
   * Madagascar
   * Mali
   * Morocco
@@ -40,29 +66,29 @@
   * Togo
 
 * National checksum algorithms for many countries have been added:
 
   * Albania
   * Bosnia and Herzegovina
   * Czech Republic
-  * East timor
+  * East Timor
   * Estonia
   * Finland
   * Iceland
-  * Mauretania
+  * Mauritania
   * Montenegro
   * North Macedonia
   * Norway
   * Poland
   * Portugal
   * Serbia
   * Slovakia
   * Slovenia
   * Spain
-  * Tunesia
+  * Tunisia
 
 * Add new banks to the list of French banks `@Natim <https://github.com/Natim>`_:
 
   * ARKEA BP Brest
   * Anytime
   * Lydia Bank
   * MEMO BANK
@@ -86,15 +112,15 @@
 
 Changed
 ~~~~~~~
 * Use enhanced IBAN/BBAN format from `Wikipedia <https://en.wikipedia.org/wiki/International_Bank_Account_Number#IBAN_formats_by_country>`_,
   since the official information from SWIFT is often inacurate.
 * The support for national checksum digits has been reimplemented.
 * The :class:`.IBAN`-class now has an additional :attr:`.IBAN.bban`-attribute, where all country
-  specific functionallity has been moved to.
+  specific functionality has been moved to.
 * Updated bank registries. Thanks to `@sh4dowb <https://github.com/sh4dowb>`_ for the Turkish banks.
 
 
 `2023.11.2`_ - 2023/11/27
 -------------------------
 Added
 ~~~~~
@@ -534,14 +560,15 @@
 -------------------------
 
 Added
 ~~~~~
 * Added :attr:`.BIC.country` and :attr:`.IBAN.country`.
 
 
+.. _2024.04.0: https://github.com/mdomke/schwifty/compare/2023.01.1...2024.04.0
 .. _2024.01.1: https://github.com/mdomke/schwifty/compare/2023.11.2...2024.01.1
 .. _2023.11.2: https://github.com/mdomke/schwifty/compare/2023.11.1...2023.11.2
 .. _2023.11.1: https://github.com/mdomke/schwifty/compare/2023.11.0...2023.11.1
 .. _2023.11.0: https://github.com/mdomke/schwifty/compare/2023.10.0...2023.11.0
 .. _2023.10.0: https://github.com/mdomke/schwifty/compare/2023.09.0...2023.10.0
 .. _2023.09.0: https://github.com/mdomke/schwifty/compare/2023.06.0...2023.09.0
 .. _2023.06.0: https://github.com/mdomke/schwifty/compare/2023.03.0...2023.06.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `schwifty-2024.1.1.post0/devbox.lock` & `schwifty-2024.4.0/devbox.lock`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'packages'": "{replace: OrderedDict([('python@3.12', OrderedDict([('last_modified', "*

 * *               "'2023-12-13T22:54:10Z'), ('plugin_version', '0.0.3'), ('resolved', "*

 * *               "'github:NixOS/nixpkgs/fd04bea4cbf76f86f244b9e2549fca066db8ddff#python312'), "*

 * *               "('source', 'devbox-search'), ('version', '3.12.1'), ('systems', "*

 * *               "OrderedDict([('aarch64-darwin', OrderedDict([('store_path', "*

 * *               "'/nix/store/ph2c8v66fnn59bjd3n6gf6ijby35fy97-python3-3.12.1')])), "*

 * *  […]*

```diff
@@ -1,26 +1,26 @@
 {
     "lockfile_version": "1",
     "packages": {
-        "python@3.11": {
-            "last_modified": "2023-11-17T14:14:56Z",
+        "python@3.12": {
+            "last_modified": "2023-12-13T22:54:10Z",
             "plugin_version": "0.0.3",
-            "resolved": "github:NixOS/nixpkgs/a71323f68d4377d12c04a5410e214495ec598d4c#python3",
+            "resolved": "github:NixOS/nixpkgs/fd04bea4cbf76f86f244b9e2549fca066db8ddff#python312",
             "source": "devbox-search",
             "systems": {
                 "aarch64-darwin": {
-                    "store_path": "/nix/store/ai4hd8f1xhr0rfjdr17bxx1rwi42sx97-python3-3.11.6"
+                    "store_path": "/nix/store/ph2c8v66fnn59bjd3n6gf6ijby35fy97-python3-3.12.1"
                 },
                 "aarch64-linux": {
-                    "store_path": "/nix/store/7ahkv87jj59z90yal5dcrgagz58cqmz6-python3-3.11.6"
+                    "store_path": "/nix/store/crw8ipyh7njx484zssl8h2cw4kg1dr4r-python3-3.12.1"
                 },
                 "x86_64-darwin": {
-                    "store_path": "/nix/store/dc4xnyqi2kh25f1c74dfczxw95anbhhr-python3-3.11.6"
+                    "store_path": "/nix/store/fl15fnagapcq8csawqpbbifjlhx7wxgg-python3-3.12.1"
                 },
                 "x86_64-linux": {
-                    "store_path": "/nix/store/qp5zys77biz7imbk6yy85q5pdv7qk84j-python3-3.11.6"
+                    "store_path": "/nix/store/3vcbpxqx9lq044manf6jnkri8krifz5s-python3-3.12.1"
                 }
             },
-            "version": "3.11.6"
+            "version": "3.12.1"
         }
     }
 }
```

### Comparing `schwifty-2024.1.1.post0/.github/workflows/lint-and-test.yml` & `schwifty-2024.4.0/.github/workflows/lint-and-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,44 +7,44 @@
     branches: [main]
 
 jobs:
   lint-docs:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: pip install hatch
       - name: Lint documentation
         run: hatch run lint:docs
 
   lint-style:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: pip install hatch
       - name: Lint style
         run: hatch run lint:style
 
   lint-typing:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: pip install hatch
       - name: Lint typing
         run: hatch run lint:typing
 
   test:
     runs-on: ubuntu-latest
```

### Comparing `schwifty-2024.1.1.post0/.github/workflows/publish.yml` & `schwifty-2024.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/Makefile` & `schwifty-2024.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/source/api.rst` & `schwifty-2024.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/source/conf.py` & `schwifty-2024.4.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import sys
 from datetime import datetime
+from typing import Any
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath("../.."))
 
-import schwifty  # noqa
+import schwifty
 
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
@@ -50,15 +51,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = []
+exclude_patterns: list[str] = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -89,15 +90,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
+html_theme_options: dict[str, Any] = {
     # "sidebar_hide_name": True,
     # "github_user": "mdomke",
     # "github_repo": "schwifty",
     # "description": "A library for parsing and validating IBANs and BICs",
     # "sidebar_collapse": False,
 }
```

### Comparing `schwifty-2024.1.1.post0/docs/source/examples.rst` & `schwifty-2024.4.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/source/ilikewhatugot.png` & `schwifty-2024.4.0/docs/source/ilikewhatugot.png`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/source/index.rst` & `schwifty-2024.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/docs/source/troubleshooting.rst` & `schwifty-2024.4.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bban.py` & `schwifty-2024.4.0/schwifty/bban.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,14 +68,21 @@
         self.country_code = country_code
 
     @classmethod
     def from_components(cls, country_code: str, **values: str) -> BBAN:
         """Generate a BBAN from its national components.
 
         The currently supported ``values`` are ``bank_code``, ``branch_code`` and ``account_code``.
+
+        Args:
+            country_code (str): The ISO 3166 alpha-2 country code.
+            values: The country specific BBAN components.
+
+        Raises:
+            InvalidAccountCode: If the account code does not meet the national requirements.
         """
         spec: dict[str, Any] = _get_bban_spec(country_code)
         if "positions" not in spec:
             raise exceptions.SchwiftyException(f"BBAN generation for {country_code} not supported")
 
         bank_code_length: int = calc_value_length(spec, Component.BANK_CODE)
         branch_code_length: int = calc_value_length(spec, Component.BRANCH_CODE)
@@ -229,7 +236,10 @@
         """str or None: The name of the bank associated with the IBAN bank code.
 
         Examples:
             >>> IBAN('DE89370400440532013000').bank_short_name
             'Commerzbank Köln'
         """
         return None if self.bank is None else self.bank["short_name"]
+
+
+registry.build_index("bank", "country", key="country_code", accumulate=True)
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bic.py` & `schwifty-2024.4.0/schwifty/bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/common.py` & `schwifty-2024.4.0/schwifty/common.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/exceptions.py` & `schwifty-2024.4.0/schwifty/exceptions.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/iban.py` & `schwifty-2024.4.0/schwifty/iban.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,41 @@
     def __init__(self, iban: str, allow_invalid: bool = False, validate_bban: bool = False) -> None:
         super().__init__()
         self.bban = BBAN(self.country_code, self._get_slice(start=4))
         if not allow_invalid:
             self.validate(validate_bban)
 
     @classmethod
+    def from_bban(
+        cls,
+        country_code: str,
+        bban: str | BBAN,
+        allow_invalid: bool = False,
+        validate_bban: bool = False,
+    ) -> IBAN:
+        """Create an IBAN from a given BBAN.
+
+        This will automatically calculate the IBAN checksum digits.
+
+        Args:
+            country_code (str): The ISO 3166 alpha-2 country code.
+            bban (str or BBAN): The national Basic Bank Account Number.
+            allow_invalid (bool): If set to `True` IBAN validation is skipped on instantiation.
+            validate_bban (bool): If set to `True` also check the country specific checksum.
+
+        .. versionadded:: 2024.01.2
+        """
+        checksum_algo = ISO7064_mod97_10()
+        return cls(
+            country_code + checksum_algo.compute([bban, country_code]) + bban,
+            allow_invalid=allow_invalid,
+            validate_bban=validate_bban,
+        )
+
+    @classmethod
     def generate(
         cls, country_code: str, bank_code: str, account_code: str, branch_code: str = ""
     ) -> IBAN:
         """Generate an IBAN from it's components.
 
         If the bank-code and/or account-number have less digits than required by their
         country specific representation, the respective component is padded with zeros.
@@ -96,30 +123,34 @@
                 'DE89 3704 0044 0532 0130 00'
 
         Args:
             country_code (str): The ISO 3166 alpha-2 country code.
             bank_code (str): The country specific bank-code.
             account_code (str): The customer specific account-code.
 
+        Raises:
+            InvalidAccountCode: If the account code does not meet the national requirements.
+
         .. versionchanged:: 2020.08.3
             Added the `branch_code` parameter to allow the branch code (or sort code) to be
             specified independently.
 
         .. versionchanged:: 2021.05.2
             Added support for generating the country specific checksum of the BBAN for Belgian
             banks.
         """
-        bban = BBAN.from_components(
+        return cls.from_bban(
             country_code,
-            bank_code=bank_code,
-            branch_code=branch_code,
-            account_code=account_code,
+            BBAN.from_components(
+                country_code,
+                bank_code=bank_code,
+                branch_code=branch_code,
+                account_code=account_code,
+            ),
         )
-        checksum_algo = ISO7064_mod97_10()
-        return cls(country_code + checksum_algo.compute([bban, country_code]) + bban)
 
     def validate(self, validate_bban: bool = False) -> bool:
         """Validate the structural integrity of this IBAN.
 
         This function will verify the country specific format as well as the Luhn checksum in the
         3rd and 4th position of the IBAN. For some countries (currently Belgium, Germany and Italy)
         it will also verify the correctness of the country specific checksum within the BBAN if the
```

### Comparing `schwifty-2024.1.1.post0/schwifty/registry.py` & `schwifty-2024.4.0/schwifty/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,86 +4,94 @@
 import json
 import pathlib
 import sys
 from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Union
 
 
 try:
-    from importlib.abc import Traversable
     from importlib.resources import files
+    from importlib.resources.abc import Traversable
 except ImportError:
     from importlib_resources import files  # type: ignore
     from importlib_resources.abc import Traversable  # type: ignore
 
 
-_registry: dict[str, dict | list[dict]] = {}
+Key = Union[str, tuple]
+Value = Union[Dict[Key, Any], List[Dict[Key, Any]]]
 
+_registry: dict[Key, Value] = {}
 
-def merge_dicts(left: dict, right: dict) -> dict:
+
+def merge_dicts(left: dict[Key, Any], right: dict[Key, Any]) -> dict[Key, Any]:
     merged = {}
     for key in frozenset(right) & frozenset(left):
         left_value, right_value = left[key], right[key]
         if isinstance(left_value, dict) and isinstance(right_value, dict):
             merged[key] = merge_dicts(left_value, right_value)
         else:
             merged[key] = right_value
 
     for key, value in itertools.chain(left.items(), right.items()):
         if key not in merged:
             merged[key] = value
     return merged
 
 
-def has(name: str) -> bool:
+def has(name: Key) -> bool:
     return name in _registry
 
 
-def get(name: str) -> dict | list[dict]:
-    if not has(name):
-        data = None
-        package_path: Traversable | Path
-        if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
-            package_path = Path(sys._MEIPASS)
-        else:
-            package_path = files(__package__)
-        directory = package_path / f"{name}_registry"
-        assert isinstance(directory, pathlib.Path)
-        for entry in sorted(directory.glob("*.json")):
-            with entry.open(encoding="utf-8") as fp:
-                chunk = json.load(fp)
-                if data is None:
-                    data = chunk
-                elif isinstance(data, list):
-                    data.extend(chunk)
-                elif isinstance(data, dict):
-                    data = merge_dicts(data, chunk)
-        if data is None:
-            raise ValueError(f"Failed to load registry {name}")
-        save(name, data)
-    return _registry[name]
+def get(name: Key) -> Value:
+    if has(name):
+        return _registry[name]
+
+    data = None
+    package_path: Traversable | Path
+    if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
+        package_path = Path(sys._MEIPASS)
+    else:
+        package_path = files(__package__)
+    directory = package_path / f"{name}_registry"
+    assert isinstance(directory, pathlib.Path)
+    for entry in sorted(directory.glob("*.json")):
+        with entry.open(encoding="utf-8") as fp:
+            chunk = json.load(fp)
+            if data is None:
+                data = chunk
+            elif isinstance(data, list):
+                data.extend(chunk)
+            elif isinstance(data, dict):
+                data = merge_dicts(data, chunk)
+    if data is None:
+        raise ValueError(f"Failed to load registry {name}")
+    return save(name, data)
 
 
-def save(name: str, data: dict | list[dict]) -> None:
+def save(name: Key, data: Value) -> Value:
     _registry[name] = data
+    return data
 
 
 def build_index(
     base_name: str,
     index_name: str,
-    key: str | tuple,
+    key: str | tuple[str, ...],
     accumulate: bool = False,
     **predicate: Any,
 ) -> None:
-    def make_key(entry: dict) -> tuple | str:
+    def make_key(entry: dict[Key, Any]) -> tuple | str:
         return tuple(entry[k] for k in key) if isinstance(key, tuple) else entry[key]
 
-    def match(entry: dict) -> bool:
+    def match(entry: dict[Key, Any]) -> bool:
         return all(entry[key] == value for key, value in predicate.items())
 
     base = get(base_name)
     assert isinstance(base, list)
     if accumulate:
         data = defaultdict(list)
         for entry in base:
@@ -96,15 +104,15 @@
         for entry in base:
             if not match(entry):
                 continue
             entries[make_key(entry)] = entry
         save(index_name, entries)
 
 
-def manipulate(name: str, func: Callable) -> None:
+def manipulate(name: Key, func: Callable) -> None:
     registry = get(name)
     if isinstance(registry, dict):
         for key, value in registry.items():
             registry[key] = func(key, value)
     elif isinstance(registry, list):
         registry = [func(item) for item in registry]
     save(name, registry)
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/README.md` & `schwifty-2024.4.0/schwifty/bank_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_at.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_at.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ba.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ba.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_be.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_be.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ch.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ch.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_cz.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_cz.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9066666666666668%*

 * *Differences: {'0': "{'name': 'Komerční banka, a.s.', 'short_name': 'Komerční banka, a.s.'}",*

 * * '1': "{'name': 'Československá obchodní banka, a. s.', 'short_name': 'Československá obchodní "*

 * *      "banka, a. s.'}",*

 * * '10': "{'name': 'Artesa, spořitelní družstvo', 'short_name': 'Artesa, spořitelní družstvo'}",*

 * * '12': "{'name': 'NEY spořitelní družstvo', 'short_name': 'NEY spořitelní družstvo'}",*

 * * '13': "{'name': 'Podnikatelská družstevní záložna', 'short_name': 'Podnikatelská družstevní "*

 * *       "záložna'}",*

 * * '14': "{'name […]*

```diff
@@ -1,127 +1,127 @@
 [
     {
         "bank_code": "0100",
         "bic": "KOMBCZPP",
         "country_code": "CZ",
-        "name": "Komer\u00c4\u008dn\u00c3\u00ad banka, a.s.",
+        "name": "Komer\u010dn\u00ed banka, a.s.",
         "primary": true,
-        "short_name": "Komer\u00c4\u008dn\u00c3\u00ad banka, a.s."
+        "short_name": "Komer\u010dn\u00ed banka, a.s."
     },
     {
         "bank_code": "0300",
         "bic": "CEKOCZPP",
         "country_code": "CZ",
-        "name": "\u00c4\u008ceskoslovensk\u00c3\u00a1 obchodn\u00c3\u00ad banka, a. s.",
+        "name": "\u010ceskoslovensk\u00e1 obchodn\u00ed banka, a. s.",
         "primary": true,
-        "short_name": "\u00c4\u008ceskoslovensk\u00c3\u00a1 obchodn\u00c3\u00ad banka, a. s."
+        "short_name": "\u010ceskoslovensk\u00e1 obchodn\u00ed banka, a. s."
     },
     {
         "bank_code": "0600",
         "bic": "AGBACZPP",
         "country_code": "CZ",
         "name": "MONETA Money Bank, a.s.",
         "primary": true,
         "short_name": "MONETA Money Bank, a.s."
     },
     {
         "bank_code": "0710",
         "bic": "CNBACZPP",
         "country_code": "CZ",
-        "name": "\u00c4\u008cESK\u00c3\u0081 N\u00c3\u0081RODN\u00c3\u008d BANKA",
+        "name": "\u010cESK\u00c1 N\u00c1RODN\u00cd BANKA",
         "primary": true,
-        "short_name": "\u00c4\u008cESK\u00c3\u0081 N\u00c3\u0081RODN\u00c3\u008d BANKA"
+        "short_name": "\u010cESK\u00c1 N\u00c1RODN\u00cd BANKA"
     },
     {
         "bank_code": "0800",
         "bic": "GIBACZPX",
         "country_code": "CZ",
-        "name": "\u00c4\u008cesk\u00c3\u00a1 spo\u00c5\u0099itelna, a.s.",
+        "name": "\u010cesk\u00e1 spo\u0159itelna, a.s.",
         "primary": true,
-        "short_name": "\u00c4\u008cesk\u00c3\u00a1 spo\u00c5\u0099itelna, a.s."
+        "short_name": "\u010cesk\u00e1 spo\u0159itelna, a.s."
     },
     {
         "bank_code": "2010",
         "bic": "FIOBCZPP",
         "country_code": "CZ",
         "name": "Fio banka, a.s.",
         "primary": true,
         "short_name": "Fio banka, a.s."
     },
     {
         "bank_code": "2060",
         "bic": "CITFCZPP",
         "country_code": "CZ",
-        "name": "Citfin, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo",
+        "name": "Citfin, spo\u0159iteln\u00ed dru\u017estvo",
         "primary": true,
-        "short_name": "Citfin, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo"
+        "short_name": "Citfin, spo\u0159iteln\u00ed dru\u017estvo"
     },
     {
         "bank_code": "2070",
         "bic": "MPUBCZPP",
         "country_code": "CZ",
         "name": "TRINITY BANK a.s.",
         "primary": true,
         "short_name": "TRINITY BANK a.s."
     },
     {
         "bank_code": "2100",
         "bic": "",
         "country_code": "CZ",
-        "name": "Hypote\u00c4\u008dn\u00c3\u00ad banka, a.s.",
+        "name": "\u010cSOB Hypote\u010dn\u00ed banka, a.s.",
         "primary": true,
-        "short_name": "Hypote\u00c4\u008dn\u00c3\u00ad banka, a.s."
+        "short_name": "\u010cSOB Hypote\u010dn\u00ed banka, a.s."
     },
     {
         "bank_code": "2200",
         "bic": "",
         "country_code": "CZ",
-        "name": "Pen\u00c4\u009b\u00c5\u00ben\u00c3\u00ad d\u00c5\u00afm, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo",
+        "name": "Pen\u011b\u017en\u00ed d\u016fm, spo\u0159iteln\u00ed dru\u017estvo",
         "primary": true,
-        "short_name": "Pen\u00c4\u009b\u00c5\u00ben\u00c3\u00ad d\u00c5\u00afm, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo"
+        "short_name": "Pen\u011b\u017en\u00ed d\u016fm, spo\u0159iteln\u00ed dru\u017estvo"
     },
     {
         "bank_code": "2220",
         "bic": "ARTTCZPP",
         "country_code": "CZ",
-        "name": "Artesa, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo",
+        "name": "Artesa, spo\u0159iteln\u00ed dru\u017estvo",
         "primary": true,
-        "short_name": "Artesa, spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo"
+        "short_name": "Artesa, spo\u0159iteln\u00ed dru\u017estvo"
     },
     {
         "bank_code": "2250",
         "bic": "CTASCZ22",
         "country_code": "CZ",
         "name": "Banka CREDITAS a.s.",
         "primary": true,
         "short_name": "Banka CREDITAS a.s."
     },
     {
         "bank_code": "2260",
         "bic": "",
         "country_code": "CZ",
-        "name": "NEY spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo",
+        "name": "NEY spo\u0159iteln\u00ed dru\u017estvo",
         "primary": true,
-        "short_name": "NEY spo\u00c5\u0099iteln\u00c3\u00ad dru\u00c5\u00bestvo"
+        "short_name": "NEY spo\u0159iteln\u00ed dru\u017estvo"
     },
     {
         "bank_code": "2275",
         "bic": "",
         "country_code": "CZ",
-        "name": "Podnikatelsk\u00c3\u00a1 dru\u00c5\u00bestevn\u00c3\u00ad z\u00c3\u00a1lo\u00c5\u00bena",
+        "name": "Podnikatelsk\u00e1 dru\u017estevn\u00ed z\u00e1lo\u017ena",
         "primary": true,
-        "short_name": "Podnikatelsk\u00c3\u00a1 dru\u00c5\u00bestevn\u00c3\u00ad z\u00c3\u00a1lo\u00c5\u00bena"
+        "short_name": "Podnikatelsk\u00e1 dru\u017estevn\u00ed z\u00e1lo\u017ena"
     },
     {
         "bank_code": "2600",
         "bic": "CITICZPX",
         "country_code": "CZ",
-        "name": "Citibank Europe plc, organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka",
+        "name": "Citibank Europe plc, organiza\u010dn\u00ed slo\u017eka",
         "primary": true,
-        "short_name": "Citibank Europe plc, organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka"
+        "short_name": "Citibank Europe plc, organiza\u010dn\u00ed slo\u017eka"
     },
     {
         "bank_code": "2700",
         "bic": "BACXCZPP",
         "country_code": "CZ",
         "name": "UniCredit Bank Czech Republic and Slovakia, a.s.",
         "primary": true,
@@ -135,17 +135,17 @@
         "primary": true,
         "short_name": "Air Bank a.s."
     },
     {
         "bank_code": "3050",
         "bic": "BPPFCZP1",
         "country_code": "CZ",
-        "name": "BNP Paribas Personal Finance SA, od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod",
+        "name": "BNP Paribas Personal Finance SA, od\u0161t\u011bpn\u00fd z\u00e1vod",
         "primary": true,
-        "short_name": "BNP Paribas Personal Finance SA, od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod"
+        "short_name": "BNP Paribas Personal Finance SA, od\u0161t\u011bpn\u00fd z\u00e1vod"
     },
     {
         "bank_code": "3060",
         "bic": "BPKOCZPP",
         "country_code": "CZ",
         "name": "PKO BP S.A., Czech Branch",
         "primary": true,
@@ -167,17 +167,17 @@
         "primary": true,
         "short_name": "Max banka a.s."
     },
     {
         "bank_code": "4300",
         "bic": "NROZCZPP",
         "country_code": "CZ",
-        "name": "N\u00c3\u00a1rodn\u00c3\u00ad rozvojov\u00c3\u00a1 banka, a.s.",
+        "name": "N\u00e1rodn\u00ed rozvojov\u00e1 banka, a.s.",
         "primary": true,
-        "short_name": "N\u00c3\u00a1rodn\u00c3\u00ad rozvojov\u00c3\u00a1 banka, a.s."
+        "short_name": "N\u00e1rodn\u00ed rozvojov\u00e1 banka, a.s."
     },
     {
         "bank_code": "5500",
         "bic": "RZBCCZPP",
         "country_code": "CZ",
         "name": "Raiffeisenbank a.s.",
         "primary": true,
@@ -199,129 +199,129 @@
         "primary": true,
         "short_name": "PPF banka a.s."
     },
     {
         "bank_code": "6200",
         "bic": "COBACZPX",
         "country_code": "CZ",
-        "name": "COMMERZBANK Aktiengesellschaft, pobo\u00c4\u008dka Praha",
+        "name": "COMMERZBANK Aktiengesellschaft, pobo\u010dka Praha",
         "primary": true,
-        "short_name": "COMMERZBANK Aktiengesellschaft, pobo\u00c4\u008dka Praha"
+        "short_name": "COMMERZBANK Aktiengesellschaft, pobo\u010dka Praha"
     },
     {
         "bank_code": "6210",
         "bic": "BREXCZPP",
         "country_code": "CZ",
-        "name": "mBank S.A., organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka",
+        "name": "mBank S.A., organiza\u010dn\u00ed slo\u017eka",
         "primary": true,
-        "short_name": "mBank S.A., organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka"
+        "short_name": "mBank S.A., organiza\u010dn\u00ed slo\u017eka"
     },
     {
         "bank_code": "6300",
         "bic": "GEBACZPP",
         "country_code": "CZ",
-        "name": "BNP Paribas S.A., pobo\u00c4\u008dka \u00c4\u008cesk\u00c3\u00a1 republika",
+        "name": "BNP Paribas S.A., pobo\u010dka \u010cesk\u00e1 republika",
         "primary": true,
-        "short_name": "BNP Paribas S.A., pobo\u00c4\u008dka \u00c4\u008cesk\u00c3\u00a1 republika"
+        "short_name": "BNP Paribas S.A., pobo\u010dka \u010cesk\u00e1 republika"
     },
     {
         "bank_code": "6363",
         "bic": "",
         "country_code": "CZ",
         "name": "Partners Banka, a.s.",
         "primary": true,
         "short_name": "Partners Banka, a.s."
     },
     {
         "bank_code": "6700",
         "bic": "SUBACZPP",
         "country_code": "CZ",
-        "name": "V\u00c5\u00a1eobecn\u00c3\u00a1 \u00c3\u00baverov\u00c3\u00a1 banka a.s., pobo\u00c4\u008dka Praha",
+        "name": "V\u0161eobecn\u00e1 \u00faverov\u00e1 banka a.s., pobo\u010dka Praha",
         "primary": true,
-        "short_name": "V\u00c5\u00a1eobecn\u00c3\u00a1 \u00c3\u00baverov\u00c3\u00a1 banka a.s., pobo\u00c4\u008dka Praha"
+        "short_name": "V\u0161eobecn\u00e1 \u00faverov\u00e1 banka a.s., pobo\u010dka Praha"
     },
     {
         "bank_code": "6800",
         "bic": "VBOECZ2X",
         "country_code": "CZ",
         "name": "Sberbank CZ, a.s. v likvidaci",
         "primary": true,
         "short_name": "Sberbank CZ, a.s. v likvidaci"
     },
     {
         "bank_code": "7910",
         "bic": "DEUTCZPX",
         "country_code": "CZ",
-        "name": "Deutsche Bank Aktiengesellschaft Filiale Prag, organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka",
+        "name": "Deutsche Bank Aktiengesellschaft Filiale Prag, organiza\u010dn\u00ed slo\u017eka",
         "primary": true,
-        "short_name": "Deutsche Bank Aktiengesellschaft Filiale Prag, organiza\u00c4\u008dn\u00c3\u00ad slo\u00c5\u00beka"
+        "short_name": "Deutsche Bank Aktiengesellschaft Filiale Prag, organiza\u010dn\u00ed slo\u017eka"
     },
     {
         "bank_code": "7950",
         "bic": "",
         "country_code": "CZ",
-        "name": "Raiffeisen stavebn\u00c3\u00ad spo\u00c5\u0099itelna a.s.",
+        "name": "Raiffeisen stavebn\u00ed spo\u0159itelna a.s.",
         "primary": true,
-        "short_name": "Raiffeisen stavebn\u00c3\u00ad spo\u00c5\u0099itelna a.s."
+        "short_name": "Raiffeisen stavebn\u00ed spo\u0159itelna a.s."
     },
     {
         "bank_code": "7960",
         "bic": "",
         "country_code": "CZ",
-        "name": "\u00c4\u008cSOB Stavebn\u00c3\u00ad spo\u00c5\u0099itelna, a.s.",
+        "name": "\u010cSOB Stavebn\u00ed spo\u0159itelna, a.s.",
         "primary": true,
-        "short_name": "\u00c4\u008cSOB Stavebn\u00c3\u00ad spo\u00c5\u0099itelna, a.s."
+        "short_name": "\u010cSOB Stavebn\u00ed spo\u0159itelna, a.s."
     },
     {
         "bank_code": "7970",
         "bic": "",
         "country_code": "CZ",
-        "name": "MONETA Stavebn\u00c3\u00ad Spo\u00c5\u0099itelna, a.s.",
+        "name": "MONETA Stavebn\u00ed Spo\u0159itelna, a.s.",
         "primary": true,
-        "short_name": "MONETA Stavebn\u00c3\u00ad Spo\u00c5\u0099itelna, a.s."
+        "short_name": "MONETA Stavebn\u00ed Spo\u0159itelna, a.s."
     },
     {
         "bank_code": "7990",
         "bic": "",
         "country_code": "CZ",
-        "name": "Modr\u00c3\u00a1 pyramida stavebn\u00c3\u00ad spo\u00c5\u0099itelna, a.s.",
+        "name": "Modr\u00e1 pyramida stavebn\u00ed spo\u0159itelna, a.s.",
         "primary": true,
-        "short_name": "Modr\u00c3\u00a1 pyramida stavebn\u00c3\u00ad spo\u00c5\u0099itelna, a.s."
+        "short_name": "Modr\u00e1 pyramida stavebn\u00ed spo\u0159itelna, a.s."
     },
     {
         "bank_code": "8030",
         "bic": "GENOCZ21",
         "country_code": "CZ",
-        "name": "Volksbank Raiffeisenbank Nordoberpfalz eG pobo\u00c4\u008dka Cheb",
+        "name": "Volksbank Raiffeisenbank Nordoberpfalz eG pobo\u010dka Cheb",
         "primary": true,
-        "short_name": "Volksbank Raiffeisenbank Nordoberpfalz eG pobo\u00c4\u008dka Cheb"
+        "short_name": "Volksbank Raiffeisenbank Nordoberpfalz eG pobo\u010dka Cheb"
     },
     {
         "bank_code": "8040",
         "bic": "OBKLCZ2X",
         "country_code": "CZ",
-        "name": "Oberbank AG pobo\u00c4\u008dka \u00c4\u008cesk\u00c3\u00a1 republika",
+        "name": "Oberbank AG pobo\u010dka \u010cesk\u00e1 republika",
         "primary": true,
-        "short_name": "Oberbank AG pobo\u00c4\u008dka \u00c4\u008cesk\u00c3\u00a1 republika"
+        "short_name": "Oberbank AG pobo\u010dka \u010cesk\u00e1 republika"
     },
     {
         "bank_code": "8060",
         "bic": "",
         "country_code": "CZ",
-        "name": "Stavebn\u00c3\u00ad spo\u00c5\u0099itelna \u00c4\u008cesk\u00c3\u00a9 spo\u00c5\u0099itelny, a.s.",
+        "name": "Stavebn\u00ed spo\u0159itelna \u010cesk\u00e9 spo\u0159itelny, a.s.",
         "primary": true,
-        "short_name": "Stavebn\u00c3\u00ad spo\u00c5\u0099itelna \u00c4\u008cesk\u00c3\u00a9 spo\u00c5\u0099itelny, a.s."
+        "short_name": "Stavebn\u00ed spo\u0159itelna \u010cesk\u00e9 spo\u0159itelny, a.s."
     },
     {
         "bank_code": "8090",
         "bic": "CZEECZPP",
         "country_code": "CZ",
-        "name": "\u00c4\u008cesk\u00c3\u00a1 exportn\u00c3\u00ad banka, a.s.",
+        "name": "\u010cesk\u00e1 exportn\u00ed banka, a.s.",
         "primary": true,
-        "short_name": "\u00c4\u008cesk\u00c3\u00a1 exportn\u00c3\u00ad banka, a.s."
+        "short_name": "\u010cesk\u00e1 exportn\u00ed banka, a.s."
     },
     {
         "bank_code": "8150",
         "bic": "MIDLCZPP",
         "country_code": "CZ",
         "name": "HSBC Continental Europe, Czech Republic",
         "primary": true,
@@ -359,25 +359,25 @@
         "primary": true,
         "short_name": "Bank of China (CEE) Ltd. Prague Branch"
     },
     {
         "bank_code": "8255",
         "bic": "COMMCZPP",
         "country_code": "CZ",
-        "name": "Bank of Communications Co., Ltd., Prague Branch od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod",
+        "name": "Bank of Communications Co., Ltd., Prague Branch od\u0161t\u011bpn\u00fd z\u00e1vod",
         "primary": true,
-        "short_name": "Bank of Communications Co., Ltd., Prague Branch od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod"
+        "short_name": "Bank of Communications Co., Ltd., Prague Branch od\u0161t\u011bpn\u00fd z\u00e1vod"
     },
     {
         "bank_code": "8265",
         "bic": "ICBKCZPP",
         "country_code": "CZ",
-        "name": "Industrial and Commercial Bank of China Limited, Prague Branch, od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod",
+        "name": "Industrial and Commercial Bank of China Limited, Prague Branch, od\u0161t\u011bpn\u00fd z\u00e1vod",
         "primary": true,
-        "short_name": "Industrial and Commercial Bank of China Limited, Prague Branch, od\u00c5\u00a1t\u00c4\u009bpn\u00c3\u00bd z\u00c3\u00a1vod"
+        "short_name": "Industrial and Commercial Bank of China Limited, Prague Branch, od\u0161t\u011bpn\u00fd z\u00e1vod"
     },
     {
         "bank_code": "8280",
         "bic": "BEFKCZP1",
         "country_code": "CZ",
         "name": "B-Efekt a.s.",
         "primary": true,
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_de.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_de.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ee.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ee.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_es.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_es.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982486865148862%*

 * *Differences: {'insert': "[(570, OrderedDict([('country_code', 'ES'), ('primary', True), ('bank_code', '1583'), "*

 * *           "('bic', 'REVOESM2XXX'), ('name', 'REVOLUT BANK UAB'), ('short_name', 'REVOLUT BANK "*

 * *           "UAB')]))]"}*

```diff
@@ -4554,9 +4554,17 @@
     {
         "bank_code": "2405",
         "bic": "",
         "country_code": "ES",
         "name": "CAIXA D'ESTALVIS LAIETANA",
         "primary": true,
         "short_name": "CAIXA LAIETANA"
+    },
+    {
+        "bank_code": "1583",
+        "bic": "REVOESM2XXX",
+        "country_code": "ES",
+        "name": "REVOLUT BANK UAB",
+        "primary": true,
+        "short_name": "REVOLUT BANK UAB"
     }
 ]
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_fi.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_fi.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ge.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ge.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_hr.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_hr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_hu.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_hu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_it.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_kz.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_kz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lt.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_lt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lu.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_lu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_lv.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_lv.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_md.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_md.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_nl.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_nl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_no.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_no.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_pl.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_pl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ro.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ro.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_rs.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_rs.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_se.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_se.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_si.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_si.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_sk.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_sk.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/generated_ua.json` & `schwifty-2024.4.0/schwifty/bank_registry/generated_ua.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ad.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_ad.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ae.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_ae.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_bg.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_bg.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_cr.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_cr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_cy.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_cy.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9290780141843968%*

 * *Differences: {'0': "{'bank_code': ''}",*

 * * '10': "{'bank_code': ''}",*

 * * '11': "{'bank_code': ''}",*

 * * '12': "{'bank_code': ''}",*

 * * '13': "{'bank_code': ''}",*

 * * '14': "{'bank_code': ''}",*

 * * '15': "{'bank_code': ''}",*

 * * '16': "{'bank_code': ''}",*

 * * '17': "{'bank_code': ''}",*

 * * '18': "{'bank_code': ''}",*

 * * '2': "{'bank_code': ''}",*

 * * '20': "{'bank_code': ''}",*

 * * '21': "{'bank_code': ''}",*

 * * '24': "{'bank_code': ''}",*

 * * '25': "{'bank_code': ''}",*

 * * '26': "{'bank_code': ''}",*

 * * '27': "{'bank_code': ''}",*

 * * '28': "{'bank_code': ''}",*

 * * '29': "{' […]*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "bank_code": "ALFA",
+        "bank_code": "",
         "bic": "ALFACY2NXXX",
         "country_code": "CY",
         "name": "ALFA CAPITAL HOLDINGS (CYPRUS) LIMITED",
         "primary": true,
         "short_name": "ALFA CAPITAL HOLDINGS"
     },
     {
@@ -12,23 +12,23 @@
         "bic": "ABKLCY2N",
         "country_code": "CY",
         "name": "ALPHA BANK CYPRUS LTD",
         "primary": true,
         "short_name": "ALPHA BANK CYPRUS"
     },
     {
-        "bank_code": "ANCO",
+        "bank_code": "",
         "bic": "ANCOCY2NXXX",
         "country_code": "CY",
         "name": "ANCORIA BANK LTD",
         "primary": true,
         "short_name": "ANCORIA BANK"
     },
     {
-        "bank_code": "AJIB",
+        "bank_code": "",
         "bic": "AJIBCY2IXXX",
         "country_code": "CY",
         "name": "ARAB JORDAN INVESTMENT BANK",
         "primary": true,
         "short_name": "ARAB JORDAN INVESTMENT BANK"
     },
     {
@@ -36,23 +36,23 @@
         "bic": "PIRBCY2N",
         "country_code": "CY",
         "name": "ASTROBANK PUBLIC COMPANY LIMITED",
         "primary": true,
         "short_name": "ASTROBANK PUBLIC COMPANY"
     },
     {
-        "bank_code": "ATON",
+        "bank_code": "",
         "bic": "ATONCY2NXXX",
         "country_code": "CY",
         "name": "ATONLINE LIMITED",
         "primary": true,
         "short_name": "ATONLINE"
     },
     {
-        "bank_code": "BABE",
+        "bank_code": "",
         "bic": "BABECY2NXXX",
         "country_code": "CY",
         "name": "BANK OF BEIRUT S.A.L CYPRUS BRANCH",
         "primary": true,
         "short_name": "BANK OF BEIRUT S.A.L"
     },
     {
@@ -60,95 +60,95 @@
         "bic": "BCYPCY2N",
         "country_code": "CY",
         "name": "BANK OF CYPRUS PUBLIC COMPANY LIMITED",
         "primary": true,
         "short_name": "BANK OF CYPRUS PUBLIC COMPANY"
     },
     {
-        "bank_code": "EUMO",
+        "bank_code": "",
         "bic": "EUMOCY2IXXX",
         "country_code": "CY",
         "name": "BANQUE BEMO SAL",
         "primary": true,
         "short_name": "BANQUE BEMO SAL"
     },
     {
-        "bank_code": "SBAA",
+        "bank_code": "",
         "bic": "SBAACY2IXXX",
         "country_code": "CY",
         "name": "BANQUE SBA - INTERNATIONAL BANKING UNIT",
         "primary": true,
         "short_name": "BANQUE SBA"
     },
     {
-        "bank_code": "BBAC",
+        "bank_code": "",
         "bic": "BBACCY2NXXX",
         "country_code": "CY",
         "name": "BBAC SAL LIMASSOL BRANCH",
         "primary": true,
         "short_name": "BBAC SAL LIMASSOL BRANCH"
     },
     {
-        "bank_code": "BLOM",
+        "bank_code": "",
         "bic": "BLOMCY2IXXX",
         "country_code": "CY",
         "name": "BLOM BANK S.A.L.",
         "primary": true,
         "short_name": "BLOM BANK"
     },
     {
-        "bank_code": "BYBA",
+        "bank_code": "",
         "bic": "BYBACY2IXXX",
         "country_code": "CY",
         "name": "BYBLOS BANK S.A.L. (IBU)",
         "primary": true,
         "short_name": "BYBLOS BANK"
     },
     {
-        "bank_code": "CBCY",
+        "bank_code": "",
         "bic": "CBCYCY2NXXX",
         "country_code": "CY",
         "name": "CENTRAL BANK OF CYPRUS",
         "primary": true,
         "short_name": "CENTRAL BANK OF CYPRUS"
     },
     {
-        "bank_code": "CECB",
+        "bank_code": "",
         "bic": "CECBCY2NXXX",
         "country_code": "CY",
         "name": "CENTRAL COOPERATIVE BANK PLC",
         "primary": true,
         "short_name": "CENTRAL COOPERATIVE BANK"
     },
     {
-        "bank_code": "CLIB",
+        "bank_code": "",
         "bic": "CLIBCY2LXXX",
         "country_code": "CY",
         "name": "CREDIT LIBANAIS S.A.L",
         "primary": true,
         "short_name": "CREDIT LIBANAIS"
     },
     {
-        "bank_code": "CYDB",
+        "bank_code": "",
         "bic": "CYDBCY2NXXX",
         "country_code": "CY",
         "name": "CYPRUS DEVELOPMENT BANK PUBLIC COMPANY LTD",
         "primary": true,
         "short_name": "CYPRUS DEVELOPMENT BANK PUBLIC COMPANY"
     },
     {
-        "bank_code": "XCYS",
+        "bank_code": "",
         "bic": "XCYSCY2NXXX",
         "country_code": "CY",
         "name": "CYPRUS STOCK EXCHANGE",
         "primary": true,
         "short_name": "CYPRUS STOCK EXCHANGE"
     },
     {
-        "bank_code": "ECBX",
+        "bank_code": "",
         "bic": "ECBXCY2NXXX",
         "country_code": "CY",
         "name": "ECOMMBX LIMITED",
         "primary": true,
         "short_name": "ECOMMBX"
     },
     {
@@ -156,23 +156,23 @@
         "bic": "ERBKCY2N",
         "country_code": "CY",
         "name": "EUROBANK CYPRUS LTD",
         "primary": true,
         "short_name": "EUROBANK CYPRUS"
     },
     {
-        "bank_code": "FINV",
+        "bank_code": "",
         "bic": "FINVCY2NXXX",
         "country_code": "CY",
         "name": "FIRST INVESTMENT BANK CYPRUS INTERNATIONAL BANKING UNIT",
         "primary": true,
         "short_name": "FIRST INVESTMENT BANK CYPRUS INTERNATIONAL BANKING UNIT"
     },
     {
-        "bank_code": "GPBF",
+        "bank_code": "",
         "bic": "GPBFCY2LXXX",
         "country_code": "CY",
         "name": "GPB FINANCIAL SERVICES LIMITED",
         "primary": true,
         "short_name": "GPB FINANCIAL SERVICES"
     },
     {
@@ -188,183 +188,183 @@
         "bic": "HEBACY2N",
         "country_code": "CY",
         "name": "HELLENIC BANK PUBLIC COMPANY LTD (FORMERLY CYPRUS COOPERATIVE BANK LTD)",
         "primary": true,
         "short_name": "HELLENIC BANK PUBLIC COMPANY"
     },
     {
-        "bank_code": "HFIC",
+        "bank_code": "",
         "bic": "HFICCY2NXXX",
         "country_code": "CY",
         "name": "HOUSING FINANCE CORPORATION",
         "primary": true,
         "short_name": "HOUSING FINANCE CORPORATION"
     },
     {
-        "bank_code": "INLE",
+        "bank_code": "",
         "bic": "INLECY2LXXX",
         "country_code": "CY",
         "name": "IBL BANK, SAL",
         "primary": true,
         "short_name": "IBL BANK, SAL"
     },
     {
-        "bank_code": "ISEM",
+        "bank_code": "",
         "bic": "ISEMCY22XXX",
         "country_code": "CY",
         "name": "ISXPAY",
         "primary": true,
         "short_name": "ISXPAY"
     },
     {
-        "bank_code": "JCCP",
+        "bank_code": "",
         "bic": "JCCPCY2NXXX",
         "country_code": "CY",
         "name": "JCC PAYMENT SYSTEMS LTD",
         "primary": true,
         "short_name": "JCC PAYMENT SYSTEMS"
     },
     {
-        "bank_code": "JONB",
+        "bank_code": "",
         "bic": "JONBCY2IXXX",
         "country_code": "CY",
         "name": "JORDAN AHLI BANK PLC",
         "primary": true,
         "short_name": "JORDAN AHLI BANK"
     },
     {
-        "bank_code": "JKBA",
+        "bank_code": "",
         "bic": "JKBACY2LXXX",
         "country_code": "CY",
         "name": "JORDAN KUWAIT BANK PLC",
         "primary": true,
         "short_name": "JORDAN KUWAIT BANK"
     },
     {
-        "bank_code": "LGBA",
+        "bank_code": "",
         "bic": "LGBACY2LXXX",
         "country_code": "CY",
         "name": "LEBANON AND GULF BANK S.A.L. - LARNACA BRANCH",
         "primary": true,
         "short_name": "LGB BANK S.A.L."
     },
     {
-        "bank_code": "MEIP",
+        "bank_code": "",
         "bic": "MEIPCY22XXX",
         "country_code": "CY",
         "name": "MERITKAPITAL LIMITED",
         "primary": true,
         "short_name": "MERITKAPITAL"
     },
     {
-        "bank_code": "ETHN",
+        "bank_code": "",
         "bic": "ETHNCY2NXXX",
         "country_code": "CY",
         "name": "NATIONAL BANK OF GREECE (CYPRUS) LTD.",
         "primary": true,
         "short_name": "NATIONAL BANK OF GREECE"
     },
     {
-        "bank_code": "OMFV",
+        "bank_code": "",
         "bic": "OMFVCY2NXXX",
         "country_code": "CY",
         "name": "OMEGA FUNDS INVESTMENT LIMITED",
         "primary": true,
         "short_name": "OMEGA FUNDS INVESTMENT"
     },
     {
-        "bank_code": "PBAN",
+        "bank_code": "",
         "bic": "PBANCY2NXXX",
         "country_code": "CY",
         "name": "PRIVATBANK, CYPRUS BRANCH",
         "primary": true,
         "short_name": "PRIVATBANK"
     },
     {
-        "bank_code": "RCBL",
+        "bank_code": "",
         "bic": "RCBLCY2IXXX",
         "country_code": "CY",
         "name": "RCB BANK LTD",
         "primary": true,
         "short_name": "RCB BANK"
     },
     {
-        "bank_code": "LGBA",
+        "bank_code": "",
         "bic": "LGBACY2LXXX",
         "country_code": "CY",
         "name": "RENAISSANCE SECURITIES (CYPRUS) LIMITED",
         "primary": true,
         "short_name": "RENAISSANCE SECURITIES"
     },
     {
-        "bank_code": "RNIN",
+        "bank_code": "",
         "bic": "RNINCY2NXXX",
         "country_code": "CY",
         "name": "RONIN EUROPE LIMITED",
         "primary": true,
         "short_name": "RONIN EUROPE"
     },
     {
-        "bank_code": "SEPM",
+        "bank_code": "",
         "bic": "SEPMCY2NXXX",
         "country_code": "CY",
         "name": "SEPAGA E.M.I. LTD",
         "primary": true,
         "short_name": "SEPAGA E.M.I."
     },
     {
-        "bank_code": "TDIN",
+        "bank_code": "",
         "bic": "TDINCY2NXXX",
         "country_code": "CY",
         "name": "SIB (CYPRUS) LIMITED",
         "primary": true,
         "short_name": "SIB"
     },
     {
-        "bank_code": "SKNN",
+        "bank_code": "",
         "bic": "SKNNCYN2XXX",
         "country_code": "CY",
         "name": "SKANESTAS INVESTMENTS LIMITED",
         "primary": true,
         "short_name": "SKANESTAS INVESTMENTS"
     },
     {
-        "bank_code": "SOGE",
+        "bank_code": "",
         "bic": "SOGECY2NXXX",
         "country_code": "CY",
         "name": "SOCIETE GENERALE CYPRUS LIMITED",
         "primary": true,
         "short_name": "SOCIETE GENERALE"
     },
     {
-        "bank_code": "TFIM",
+        "bank_code": "",
         "bic": "TFIMCY2NXXX",
         "country_code": "CY",
         "name": "TFI MARKETS LIMITED",
         "primary": true,
         "short_name": "TFI MARKETS"
     },
     {
-        "bank_code": "WARF",
+        "bank_code": "",
         "bic": "WARFCY2NXXX",
         "country_code": "CY",
         "name": "WARGAMING FINANCE LTD",
         "primary": true,
         "short_name": "WARGAMING FINANCE"
     },
     {
-        "bank_code": "WWFI",
+        "bank_code": "",
         "bic": "WWFICY2LXXX",
         "country_code": "CY",
         "name": "WISE WOLVES FINANCE LTD",
         "primary": true,
         "short_name": "WISE WOLVES FINANCE"
     },
     {
-        "bank_code": "WWPI",
+        "bank_code": "",
         "bic": "WWPICY2LXXX",
         "country_code": "CY",
         "name": "WISE WOLVES PAYMENT INSTITUTION LIMITED",
         "primary": true,
         "short_name": "WISE WOLVES PAYMENT INSTITUTION"
     },
     {
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_es.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_fr.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_fr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_gb.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_gb.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_gr.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_gr.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555557%*

 * *Differences: {'10': "{'bank_code': ''}", '6': "{'bank_code': ''}"}*

```diff
@@ -44,15 +44,15 @@
         "bic": "BNGRGRAA",
         "country_code": "GR",
         "name": "BANK OF GREECE S.A.",
         "primary": true,
         "short_name": "BANK OF GREECE"
     },
     {
-        "bank_code": "BSTD",
+        "bank_code": "",
         "bic": "BSTDGR2TXXX",
         "country_code": "GR",
         "name": "BLACK SEA TRADE AND DEVELOPMENT BANK",
         "primary": true,
         "short_name": "BLACK SEA TRADE AND DEVELOPMENT BANK"
     },
     {
@@ -76,15 +76,15 @@
         "bic": "STEOGR21XXX",
         "country_code": "GR",
         "name": "COOPERATIVE BANK OF DRAMA",
         "primary": true,
         "short_name": "COOPERATIVE BANK OF DRAMA"
     },
     {
-        "bank_code": "ENCH",
+        "bank_code": "",
         "bic": "ENCHGRAAXXX",
         "country_code": "GR",
         "name": "ENEX CLEARING HOUSE S.A.",
         "primary": true,
         "short_name": "ENEX CLEARING HOUSE"
     },
     {
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_ie.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_ie.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_is.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_is.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_it.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_pt.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_pt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_sa.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_sa.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666683%*

 * *Differences: {'0': "{'bank_code': ''}",*

 * * '1': "{'bank_code': ''}",*

 * * '10': "{'bank_code': ''}",*

 * * '100': "{'bank_code': ''}",*

 * * '101': "{'bank_code': ''}",*

 * * '102': "{'bank_code': ''}",*

 * * '103': "{'bank_code': ''}",*

 * * '104': "{'bank_code': ''}",*

 * * '105': "{'bank_code': ''}",*

 * * '106': "{'bank_code': ''}",*

 * * '107': "{'bank_code': ''}",*

 * * '108': "{'bank_code': ''}",*

 * * '109': "{'bank_code': ''}",*

 * * '11': "{'bank_code': ''}",*

 * * '110': "{'bank_code': ''}",*

 * * '111': "{'bank_code': ''}",*

 * * '112': "{'bank_code': ''}",*

 * * '113': "{'bank_code': '' […]*

```diff
@@ -1,1034 +1,1034 @@
 [
     {
-        "bank_code": "ALQA",
+        "bank_code": "",
         "bic": "ALQASADK",
         "country_code": "SA",
         "name": "ABDULHADI ABDULLAH AL-QAHTANI SONS GROUP HOLDING COMPANY CJSC",
         "primary": true,
         "short_name": "ABDULHADI ABDULLAH AL-QAHTANI SONS GROUP HOLDING COMPANY"
     },
     {
-        "bank_code": "INMA",
+        "bank_code": "",
         "bic": "INMASARI",
         "country_code": "SA",
         "name": "AL INMA BANK",
         "primary": true,
         "short_name": "AL INMA BANK"
     },
     {
-        "bank_code": "ALRD",
+        "bank_code": "",
         "bic": "ALRDSARI",
         "country_code": "SA",
         "name": "AL RA'IDAH INVESTMENT COMPANY",
         "primary": true,
         "short_name": "AL RA'IDAH INVESTMENT COMPANY"
     },
     {
-        "bank_code": "RJHI",
+        "bank_code": "",
         "bic": "RJHISARI",
         "country_code": "SA",
         "name": "AL RAJHI BANK",
         "primary": true,
         "short_name": "AL RAJHI BANK"
     },
     {
-        "bank_code": "SAHC",
+        "bank_code": "",
         "bic": "SAHCSARI",
         "country_code": "SA",
         "name": "ALAWWAL INVEST",
         "primary": true,
         "short_name": "ALAWWAL INVEST"
     },
     {
-        "bank_code": "FANR",
+        "bank_code": "",
         "bic": "FANRSARI",
         "country_code": "SA",
         "name": "ALFANAR CO. LTD",
         "primary": true,
         "short_name": "ALFANAR CO. LTD"
     },
     {
-        "bank_code": "ALMR",
+        "bank_code": "",
         "bic": "ALMRSARI",
         "country_code": "SA",
         "name": "ALMARAI COMPANY",
         "primary": true,
         "short_name": "ALMARAI COMPANY"
     },
     {
-        "bank_code": "ARNB",
+        "bank_code": "",
         "bic": "ARNBSARI",
         "country_code": "SA",
         "name": "ARAB NATIONAL BANK",
         "primary": true,
         "short_name": "ARAB NATIONAL BANK"
     },
     {
-        "bank_code": "APIC",
+        "bank_code": "",
         "bic": "APICSADM",
         "country_code": "SA",
         "name": "ARAB PETROLEUM INVESTMENTS CORPORATION",
         "primary": true,
         "short_name": "ARAB PETROLEUM INVESTMENTS CORPORATION"
     },
     {
-        "bank_code": "AGSC",
+        "bank_code": "",
         "bic": "AGSCSARI",
         "country_code": "SA",
         "name": "ARABIAN AGRICULTURAL SERVICES COMPANY",
         "primary": true,
         "short_name": "ARABIAN AGRICULTURAL SERVICES COMPANY"
     },
     {
-        "bank_code": "ARHM",
+        "bank_code": "",
         "bic": "ARHMSADD",
         "country_code": "SA",
         "name": "ARAMCO CHEMICALS COMPANY",
         "primary": true,
         "short_name": "ARAMCO CHEMICALS COMPANY"
     },
     {
-        "bank_code": "SAPC",
+        "bank_code": "",
         "bic": "SAPCSADH",
         "country_code": "SA",
         "name": "ARAMCO TRADING COMPANY",
         "primary": true,
         "short_name": "ARAMCO TRADING COMPANY"
     },
     {
-        "bank_code": "SAPC",
+        "bank_code": "",
         "bic": "SAPCSADHAEF",
         "country_code": "SA",
         "name": "ARAMCO TRADING COMPANY",
         "primary": true,
         "short_name": "ARAMCO TRADING COMPANY"
     },
     {
-        "bank_code": "SAPC",
+        "bank_code": "",
         "bic": "SAPCSADHUKL",
         "country_code": "SA",
         "name": "ARAMCO TRADING COMPANY",
         "primary": true,
         "short_name": "ARAMCO TRADING COMPANY"
     },
     {
-        "bank_code": "SAPC",
+        "bank_code": "",
         "bic": "SAPCSADHSSG",
         "country_code": "SA",
         "name": "ARAMCO TRADING COMPANY",
         "primary": true,
         "short_name": "ARAMCO TRADING COMPANY"
     },
     {
-        "bank_code": "ALBI",
+        "bank_code": "",
         "bic": "ALBISARIDAM",
         "country_code": "SA",
         "name": "BANK AL BILAD",
         "primary": true,
         "short_name": "BANK AL BILAD"
     },
     {
-        "bank_code": "ALBI",
+        "bank_code": "",
         "bic": "ALBISARIJED",
         "country_code": "SA",
         "name": "BANK AL BILAD",
         "primary": true,
         "short_name": "BANK AL BILAD"
     },
     {
-        "bank_code": "ALBI",
+        "bank_code": "",
         "bic": "ALBISARI",
         "country_code": "SA",
         "name": "BANK AL BILAD",
         "primary": true,
         "short_name": "BANK AL BILAD"
     },
     {
-        "bank_code": "ALBI",
+        "bank_code": "",
         "bic": "ALBISARICAP",
         "country_code": "SA",
         "name": "BANK AL BILAD",
         "primary": true,
         "short_name": "BANK AL BILAD"
     },
     {
-        "bank_code": "ALBI",
+        "bank_code": "",
         "bic": "ALBISARITFC",
         "country_code": "SA",
         "name": "BANK AL BILAD",
         "primary": true,
         "short_name": "BANK AL BILAD"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE013",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE026",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE009",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE025",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE002",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE007",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE006",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE021",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE019",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE011",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE010",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJEFWR",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE016",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BJAZ",
+        "bank_code": "",
         "bic": "BJAZSAJE027",
         "country_code": "SA",
         "name": "BANK AL-JAZIRA",
         "primary": true,
         "short_name": "BANK AL-JAZIRA"
     },
     {
-        "bank_code": "BMUS",
+        "bank_code": "",
         "bic": "BMUSSARI",
         "country_code": "SA",
         "name": "BANKMUSCAT",
         "primary": true,
         "short_name": "BANKMUSCAT"
     },
     {
-        "bank_code": "BSFR",
+        "bank_code": "",
         "bic": "BSFRSARIEST",
         "country_code": "SA",
         "name": "BANQUE SAUDI FRANSI",
         "primary": true,
         "short_name": "BANQUE SAUDI FRANSI"
     },
     {
-        "bank_code": "BSFR",
+        "bank_code": "",
         "bic": "BSFRSARIWST",
         "country_code": "SA",
         "name": "BANQUE SAUDI FRANSI",
         "primary": true,
         "short_name": "BANQUE SAUDI FRANSI"
     },
     {
-        "bank_code": "BSFR",
+        "bank_code": "",
         "bic": "BSFRSARI",
         "country_code": "SA",
         "name": "BANQUE SAUDI FRANSI",
         "primary": true,
         "short_name": "BANQUE SAUDI FRANSI"
     },
     {
-        "bank_code": "BSFR",
+        "bank_code": "",
         "bic": "BSFRSARIRYD",
         "country_code": "SA",
         "name": "BANQUE SAUDI FRANSI",
         "primary": true,
         "short_name": "BANQUE SAUDI FRANSI"
     },
     {
-        "bank_code": "BSFR",
+        "bank_code": "",
         "bic": "BSFRSARIGEM",
         "country_code": "SA",
         "name": "BANQUE SAUDI FRANSI",
         "primary": true,
         "short_name": "BANQUE SAUDI FRANSI"
     },
     {
-        "bank_code": "BNPA",
+        "bank_code": "",
         "bic": "BNPASARB",
         "country_code": "SA",
         "name": "BNP PARIBAS INVESTMENT COMPANY KSA",
         "primary": true,
         "short_name": "BNP PARIBAS INVESTMENT COMPANY KSA"
     },
     {
-        "bank_code": "BNPA",
+        "bank_code": "",
         "bic": "BNPASARBWMI",
         "country_code": "SA",
         "name": "BNP PARIBAS INVESTMENT COMPANY KSA",
         "primary": true,
         "short_name": "BNP PARIBAS INVESTMENT COMPANY KSA"
     },
     {
-        "bank_code": "BNPA",
+        "bank_code": "",
         "bic": "BNPASARI",
         "country_code": "SA",
         "name": "BNP PARIBAS SAUDI ARABIA",
         "primary": true,
         "short_name": "BNP PARIBAS SAUDI ARABIA"
     },
     {
-        "bank_code": "CITI",
+        "bank_code": "",
         "bic": "CITISARI",
         "country_code": "SA",
         "name": "CITIGROUP SAUDI ARABIA",
         "primary": true,
         "short_name": "CITIGROUP SAUDI ARABIA"
     },
     {
-        "bank_code": "CITI",
+        "bank_code": "",
         "bic": "CITISARISIG",
         "country_code": "SA",
         "name": "CITIGROUP SAUDI ARABIA",
         "primary": true,
         "short_name": "CITIGROUP SAUDI ARABIA"
     },
     {
-        "bank_code": "CRES",
+        "bank_code": "",
         "bic": "CRESSARY",
         "country_code": "SA",
         "name": "CREDIT SUISSE AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "CREDIT SUISSE AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "CRES",
+        "bank_code": "",
         "bic": "CRESSARA20R",
         "country_code": "SA",
         "name": "CREDIT SUISSE SAUDI ARABIA",
         "primary": true,
         "short_name": "CREDIT SUISSE SAUDI ARABIA"
     },
     {
-        "bank_code": "CRES",
+        "bank_code": "",
         "bic": "CRESSARA",
         "country_code": "SA",
         "name": "CREDIT SUISSE SAUDI ARABIA",
         "primary": true,
         "short_name": "CREDIT SUISSE SAUDI ARABIA"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARIGES",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARI",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARA",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARAAWM",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARACUS",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARICUS",
         "country_code": "SA",
         "name": "DEUTSCHE BANK AG, RIYADH BRANCH",
         "primary": true,
         "short_name": "DEUTSCHE BANK AG, RIYADH BRANCH"
     },
     {
-        "bank_code": "DEUT",
+        "bank_code": "",
         "bic": "DEUTSARB",
         "country_code": "SA",
         "name": "DEUTSCHE SECURITIES SAUDI ARABIA",
         "primary": true,
         "short_name": "DEUTSCHE SECURITIES SAUDI ARABIA"
     },
     {
-        "bank_code": "EBIL",
+        "bank_code": "",
         "bic": "EBILSARI",
         "country_code": "SA",
         "name": "EMIRATES NBD PJSC",
         "primary": true,
         "short_name": "EMIRATES NBD PJSC"
     },
     {
-        "bank_code": "FABM",
+        "bank_code": "",
         "bic": "FABMSARI",
         "country_code": "SA",
         "name": "FIRST ABU DHABI BANK",
         "primary": true,
         "short_name": "FIRST ABU DHABI BANK"
     },
     {
-        "bank_code": "GULF",
+        "bank_code": "",
         "bic": "GULFSARI",
         "country_code": "SA",
         "name": "GULF INTERNATIONAL BANK (GIB) SAUDI ARABIA CLOSED",
         "primary": true,
         "short_name": "GULF INTERNATIONAL BANK (GIB) SAUDI ARABIA CLOSED"
     },
     {
-        "bank_code": "ICBK",
+        "bank_code": "",
         "bic": "ICBKSARI",
         "country_code": "SA",
         "name": "INDUSTRIAL AND COMMERCIAL BANK OF CHINA RIYADH BRANCH, SA",
         "primary": true,
         "short_name": "INDUSTRIAL AND COMMERCIAL BANK OF CHINA RIYADH BRANCH, SA"
     },
     {
-        "bank_code": "IENE",
+        "bank_code": "",
         "bic": "IENESADH",
         "country_code": "SA",
         "name": "INDUSTRIALIZATION AND ENERGY SERVICES CO. (TAQA)",
         "primary": true,
         "short_name": "INDUSTRIALIZATION AND ENERGY SERVICES CO. (TAQA)"
     },
     {
-        "bank_code": "ACWA",
+        "bank_code": "",
         "bic": "ACWASARI",
         "country_code": "SA",
         "name": "INTERNATIONAL CO. FOR WATER AND POWER PROJECTS",
         "primary": true,
         "short_name": "INTERNATIONAL CO. FOR WATER AND POWER PROJECTS"
     },
     {
-        "bank_code": "ITFK",
+        "bank_code": "",
         "bic": "ITFKSAJE",
         "country_code": "SA",
         "name": "INTERNATIONAL ISLAMIC TRADE FINANCE CORPORATION (MEMBER ISLAMIC DEVELOPMENT BANK GROUP)",
         "primary": true,
         "short_name": "INTERNATIONAL ISLAMIC TRADE FINANCE CORPORATION"
     },
     {
-        "bank_code": "ICDK",
+        "bank_code": "",
         "bic": "ICDKSAJE",
         "country_code": "SA",
         "name": "ISLAMIC CORPORATION FOR THE DEVELOPMENT OF THE PRIVATE SECTOR (MEMBER, ISLAMIC DEVELOPMENT BANK GROUP)",
         "primary": true,
         "short_name": "ISLAMIC CORPORATION FOR THE DEVELOPMENT OF THE PRIVATE SECTOR"
     },
     {
-        "bank_code": "ISLD",
+        "bank_code": "",
         "bic": "ISLDSAJE",
         "country_code": "SA",
         "name": "ISLAMIC DEVELOPMENT BANK",
         "primary": true,
         "short_name": "ISLAMIC DEVELOPMENT BANK"
     },
     {
-        "bank_code": "ISLD",
+        "bank_code": "",
         "bic": "ISLDSAJEICD",
         "country_code": "SA",
         "name": "ISLAMIC DEVELOPMENT BANK",
         "primary": true,
         "short_name": "ISLAMIC DEVELOPMENT BANK"
     },
     {
-        "bank_code": "ISLD",
+        "bank_code": "",
         "bic": "ISLDSAJEITF",
         "country_code": "SA",
         "name": "ISLAMIC DEVELOPMENT BANK",
         "primary": true,
         "short_name": "ISLAMIC DEVELOPMENT BANK"
     },
     {
-        "bank_code": "JPMG",
+        "bank_code": "",
         "bic": "JPMGSARY",
         "country_code": "SA",
         "name": "J.P. MORGAN SAUDI ARABIA COMPANY",
         "primary": true,
         "short_name": "J.P. MORGAN SAUDI ARABIA COMPANY"
     },
     {
-        "bank_code": "JPMG",
+        "bank_code": "",
         "bic": "JPMGSARYDCC",
         "country_code": "SA",
         "name": "J.P. MORGAN SAUDI ARABIA COMPANY",
         "primary": true,
         "short_name": "J.P. MORGAN SAUDI ARABIA COMPANY"
     },
     {
-        "bank_code": "CHAS",
+        "bank_code": "",
         "bic": "CHASSARI",
         "country_code": "SA",
         "name": "JPMORGAN CHASE BANK, N.A. RIYADH",
         "primary": true,
         "short_name": "JPMORGAN CHASE BANK, N.A. RIYADH"
     },
     {
-        "bank_code": "CHAS",
+        "bank_code": "",
         "bic": "CHASSARISAU",
         "country_code": "SA",
         "name": "JPMORGAN CHASE BANK, N.A. RIYADH",
         "primary": true,
         "short_name": "JPMORGAN CHASE BANK, N.A. RIYADH"
     },
     {
-        "bank_code": "MLSA",
+        "bank_code": "",
         "bic": "MLSASARI",
         "country_code": "SA",
         "name": "MERRILL LYNCH KINGDOM OF SAUDI ARABIA",
         "primary": true,
         "short_name": "MERRILL LYNCH KINGDOM OF SAUDI ARABIA"
     },
     {
-        "bank_code": "BOTK",
+        "bank_code": "",
         "bic": "BOTKSARI",
         "country_code": "SA",
         "name": "MUFG BANK, LTD. RIYADH BRANCH",
         "primary": true,
         "short_name": "MUFG BANK, LTD. RIYADH BRANCH"
     },
     {
-        "bank_code": "NHDI",
+        "bank_code": "",
         "bic": "NHDISAJE",
         "country_code": "SA",
         "name": "NAHDI MEDICAL COMPANY",
         "primary": true,
         "short_name": "NAHDI MEDICAL COMPANY"
     },
     {
-        "bank_code": "NBOB",
+        "bank_code": "",
         "bic": "NBOBSARI",
         "country_code": "SA",
         "name": "NATIONAL BANK OF BAHRAIN",
         "primary": true,
         "short_name": "NATIONAL BANK OF BAHRAIN"
     },
     {
-        "bank_code": "NBOK",
+        "bank_code": "",
         "bic": "NBOKSAJE",
         "country_code": "SA",
         "name": "NATIONAL BANK OF KUWAIT",
         "primary": true,
         "short_name": "NATIONAL BANK OF KUWAIT"
     },
     {
-        "bank_code": "NBPA",
+        "bank_code": "",
         "bic": "NBPASARI",
         "country_code": "SA",
         "name": "NATIONAL BANK OF PAKISTAN",
         "primary": true,
         "short_name": "NATIONAL BANK OF PAKISTAN"
     },
     {
-        "bank_code": "NBCC",
+        "bank_code": "",
         "bic": "NBCCSAJE",
         "country_code": "SA",
         "name": "NATIONAL BISCUITS AND CONFECTIONERY COMPANY",
         "primary": true,
         "short_name": "NATIONAL BISCUITS AND CONFECTIONERY COMPANY"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE615",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE101",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE613",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE555",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NCBK",
+        "bank_code": "",
         "bic": "NCBKSAJE614",
         "country_code": "SA",
         "name": "NATIONAL COMMERCIAL BANK, THE",
         "primary": true,
         "short_name": "NATIONAL COMMERCIAL BANK, THE"
     },
     {
-        "bank_code": "NAFD",
+        "bank_code": "",
         "bic": "NAFDSAJE",
         "country_code": "SA",
         "name": "NATIONAL FOOD INDUSTRIES CO. LTD",
         "primary": true,
         "short_name": "NATIONAL FOOD INDUSTRIES CO. LTD"
     },
     {
-        "bank_code": "NAIC",
+        "bank_code": "",
         "bic": "NAICSARI",
         "country_code": "SA",
         "name": "NATIONAL INDUSTRIALIZATION COMPANY",
         "primary": true,
         "short_name": "NATIONAL INDUSTRIALIZATION COMPANY"
     },
     {
-        "bank_code": "NYFT",
+        "bank_code": "",
         "bic": "NYFTSARI",
         "country_code": "SA",
         "name": "NAYIFAT FINANCE COMPANY",
         "primary": true,
         "short_name": "NAYIFAT FINANCE COMPANY"
     },
     {
-        "bank_code": "NCCO",
+        "bank_code": "",
         "bic": "NCCOSAJE",
         "country_code": "SA",
         "name": "NCB CAPITAL COMPANY",
         "primary": true,
         "short_name": "NCB CAPITAL COMPANY"
     },
     {
-        "bank_code": "OKAM",
+        "bank_code": "",
         "bic": "OKAMSARI",
         "country_code": "SA",
         "name": "OMAR KASSEM ALESAYI MARKETING CO. LIMITED",
         "primary": true,
         "short_name": "OMAR KASSEM ALESAYI MARKETING CO. LIMITED"
     },
     {
-        "bank_code": "QNBA",
+        "bank_code": "",
         "bic": "QNBASARI",
         "country_code": "SA",
         "name": "QATAR NATIONAL BANK",
         "primary": true,
         "short_name": "QATAR NATIONAL BANK"
     },
     {
-        "bank_code": "RAWA",
+        "bank_code": "",
         "bic": "RAWASADK",
         "country_code": "SA",
         "name": "RAWABI HOLDING COMPANY",
         "primary": true,
         "short_name": "RAWABI HOLDING COMPANY"
     },
     {
-        "bank_code": "RIBL",
+        "bank_code": "",
         "bic": "RIBLSARI",
         "country_code": "SA",
         "name": "RIYAD BANK",
         "primary": true,
         "short_name": "RIYAD BANK"
     },
     {
-        "bank_code": "SDCC",
+        "bank_code": "",
         "bic": "SDCCSADA",
         "country_code": "SA",
         "name": "SADARA CHEMICAL COMPANY",
         "primary": true,
         "short_name": "SADARA CHEMICAL COMPANY"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARIACS",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARIJCS",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARI",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARIRCS",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARIRCP",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMB",
+        "bank_code": "",
         "bic": "SAMBSARIRFX",
         "country_code": "SA",
         "name": "SAMBA FINANCIAL GROUP",
         "primary": true,
         "short_name": "SAMBA FINANCIAL GROUP"
     },
     {
-        "bank_code": "SAMA",
+        "bank_code": "",
         "bic": "SAMASARI",
         "country_code": "SA",
         "name": "SAUDI ARABIAN MONETARY AUTHORITY",
         "primary": true,
         "short_name": "SAUDI ARABIAN MONETARY AUTHORITY"
     },
     {
-        "bank_code": "ARAM",
+        "bank_code": "",
         "bic": "ARAMSADH",
         "country_code": "SA",
         "name": "SAUDI ARAMCO",
         "primary": true,
         "short_name": "SAUDI ARAMCO"
     },
     {
-        "bank_code": "LBRF",
+        "bank_code": "",
         "bic": "LBRFSAJD",
         "country_code": "SA",
         "name": "SAUDI ARAMCO BASE OIL COMPANY - LUBEREF",
         "primary": true,
         "short_name": "SAUDI ARAMCO BASE OIL COMPANY - LUBEREF"
     },
     {
-        "bank_code": "SRMR",
+        "bank_code": "",
         "bic": "SRMRSADB",
         "country_code": "SA",
         "name": "SAUDI ARAMCO MOBIL REFINERY COMPANY LIMITED (SAMREF)",
         "primary": true,
         "short_name": "SAUDI ARAMCO MOBIL REFINERY COMPANY LIMITED (SAMREF)"
     },
     {
-        "bank_code": "SBHQ",
+        "bank_code": "",
         "bic": "SBHQSARR",
         "country_code": "SA",
         "name": "SAUDI BASIC INDUSTRIES CORPORATION (SABIC)",
         "primary": true,
         "short_name": "SAUDI BASIC INDUSTRIES CORPORATION (SABIC)"
     },
     {
-        "bank_code": "SABB",
+        "bank_code": "",
         "bic": "SABBSARI",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE"
     },
     {
-        "bank_code": "AAAL",
+        "bank_code": "",
         "bic": "AAALSARIALK",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)"
     },
     {
-        "bank_code": "AAAL",
+        "bank_code": "",
         "bic": "AAALSARIJED",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)"
     },
     {
-        "bank_code": "AAAL",
+        "bank_code": "",
         "bic": "AAALSARI",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)"
     },
     {
-        "bank_code": "AAAL",
+        "bank_code": "",
         "bic": "AAALSARIRYD",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)"
     },
     {
-        "bank_code": "AAAL",
+        "bank_code": "",
         "bic": "AAALSARICTD",
         "country_code": "SA",
         "name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)",
         "primary": true,
         "short_name": "SAUDI BRITISH BANK, THE (FORMERLY ALAWWAL BANK)"
     },
     {
-        "bank_code": "SCHM",
+        "bank_code": "",
         "bic": "SCHMSADE",
         "country_code": "SA",
         "name": "SAUDI CHEVRON PHILLIPS CO.",
         "primary": true,
         "short_name": "SAUDI CHEVRON PHILLIPS CO."
     },
     {
-        "bank_code": "SEDP",
+        "bank_code": "",
         "bic": "SEDPSAJE",
         "country_code": "SA",
         "name": "SAUDI ECONOMIC AND DEVELOPMENT COMPANY FOR SECURITIES",
         "primary": true,
         "short_name": "SAUDI ECONOMIC AND DEVELOPMENT COMPANY FOR SECURITIES"
     },
     {
-        "bank_code": "SFCP",
+        "bank_code": "",
         "bic": "SFCPSARI",
         "country_code": "SA",
         "name": "SAUDI FRANSI CAPITAL",
         "primary": true,
         "short_name": "SAUDI FRANSI CAPITAL"
     },
     {
-        "bank_code": "SIPH",
+        "bank_code": "",
         "bic": "SIPHSADB",
         "country_code": "SA",
         "name": "SAUDI INTERNATIONAL PETROCHEMICAL CO. (SIPCHEM)",
         "primary": true,
         "short_name": "SAUDI INTERNATIONAL PETROCHEMICAL CO. (SIPCHEM)"
     },
     {
-        "bank_code": "SIBC",
+        "bank_code": "",
         "bic": "SIBCSARI",
         "country_code": "SA",
         "name": "SAUDI INVESTMENT BANK, THE",
         "primary": true,
         "short_name": "SAUDI INVESTMENT BANK, THE"
     },
     {
-        "bank_code": "SIBC",
+        "bank_code": "",
         "bic": "SIBCSARISPV",
         "country_code": "SA",
         "name": "SAUDI INVESTMENT BANK, THE",
         "primary": true,
         "short_name": "SAUDI INVESTMENT BANK, THE"
     },
     {
-        "bank_code": "STCO",
+        "bank_code": "",
         "bic": "STCOSARI",
         "country_code": "SA",
         "name": "SAUDI TELECOM COMPANY",
         "primary": true,
         "short_name": "SAUDI TELECOM COMPANY"
     },
     {
-        "bank_code": "SCCY",
+        "bank_code": "",
         "bic": "SCCYSARI",
         "country_code": "SA",
         "name": "SECURITIES CLEARING CENTER COMPANY CLOSED JOINT STOCK COMPANY",
         "primary": true,
         "short_name": "SECURITIES CLEARING CENTER COMPANY CLOSED JOINT STOCK COMPANY"
     },
     {
-        "bank_code": "TAYR",
+        "bank_code": "",
         "bic": "TAYRSARI",
         "country_code": "SA",
         "name": "SEERA GROUP HOLDING",
         "primary": true,
         "short_name": "SEERA GROUP HOLDING"
     },
     {
-        "bank_code": "SCBL",
+        "bank_code": "",
         "bic": "SCBLSAR2",
         "country_code": "SA",
         "name": "STANDARD CHARTERED BANK BRANCH",
         "primary": true,
         "short_name": "STANDARD CHARTERED BANK BRANCH"
     },
     {
-        "bank_code": "SCBL",
+        "bank_code": "",
         "bic": "SCBLSARI",
         "country_code": "SA",
         "name": "STANDARD CHARTERED CAPITAL (SAUDI ARABIA)",
         "primary": true,
         "short_name": "STANDARD CHARTERED CAPITAL (SAUDI ARABIA)"
     },
     {
-        "bank_code": "TCZB",
+        "bank_code": "",
         "bic": "TCZBSAJE",
         "country_code": "SA",
         "name": "T.C. ZIRAAT BANKASI A.S.",
         "primary": true,
         "short_name": "T.C. ZIRAAT BANKASI A.S."
     },
     {
-        "bank_code": "ICEC",
+        "bank_code": "",
         "bic": "ICECSAJE",
         "country_code": "SA",
         "name": "THE ISLAMIC CORP FOR THE INSURANCE OF INVESTMENT AND EXPORT CREDIT (MEMBER ISLAMIC DEVELOPMENT BANKGROUP)",
         "primary": true,
         "short_name": "THE ISLAMIC CORP FOR THE INSURANCE OF INVESTMENT AND EXPORT CREDIT"
     },
     {
-        "bank_code": "BARI",
+        "bank_code": "",
         "bic": "BARISARI",
         "country_code": "SA",
         "name": "THE NATIONAL SHIPPING COMPANY OF SAUDI ARABIA",
         "primary": true,
         "short_name": "THE NATIONAL SHIPPING COMPANY OF SAUDI ARABIA"
     },
     {
-        "bank_code": "SFFD",
+        "bank_code": "",
         "bic": "SFFDSARI",
         "country_code": "SA",
         "name": "THE SAUDI FUND FOR DEVELOPMENT",
         "primary": true,
         "short_name": "THE SAUDI FUND FOR DEVELOPMENT"
     },
     {
-        "bank_code": "EXTR",
+        "bank_code": "",
         "bic": "EXTRSADA",
         "country_code": "SA",
         "name": "UNITED ELECTRONICS COMPANY",
         "primary": true,
         "short_name": "UNITED ELECTRONICS COMPANY"
     },
     {
-        "bank_code": "WGIC",
+        "bank_code": "",
         "bic": "WGICSADK",
         "country_code": "SA",
         "name": "WISAYAH GLOBAL INVESTMENT COMPANY",
         "primary": true,
         "short_name": "WISAYAH GLOBAL INVESTMENT COMPANY"
     },
     {
-        "bank_code": "YASR",
+        "bank_code": "",
         "bic": "YASRSADB",
         "country_code": "SA",
         "name": "YANBU ARAMCO SINOPEC REFINING (YASREF) LIMITED",
         "primary": true,
         "short_name": "YANBU ARAMCO SINOPEC REFINING (YASREF) LIMITED"
     },
     {
-        "bank_code": "ZTHM",
+        "bank_code": "",
         "bic": "ZTHMSAJE",
         "country_code": "SA",
         "name": "ZAHID TRACTOR AND HM",
         "primary": true,
         "short_name": "ZAHID TRACTOR AND HM"
     }
 ]
```

### Comparing `schwifty-2024.1.1.post0/schwifty/bank_registry/manual_tr.json` & `schwifty-2024.4.0/schwifty/bank_registry/manual_tr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967320261437908%*

 * *Differences: {'39': "{'bank_code': '00151'}", '40': "{'bank_code': '00152'}"}*

```diff
@@ -308,23 +308,23 @@
         "bic": "BPTRTRIS",
         "country_code": "TR",
         "name": "BankPozitif Kredi ve Kalk\u0131nma Bankas\u0131 A.\u015e.",
         "primary": true,
         "short_name": "BankPozitif Kredi ve Kalk\u0131nma Bankas\u0131 A.\u015e."
     },
     {
-        "bank_code": "0151",
+        "bank_code": "00151",
         "bic": "YATITRIS",
         "country_code": "TR",
         "name": "D Yat\u0131r\u0131m Bankas\u0131 A.\u015e.",
         "primary": true,
         "short_name": "D Yat\u0131r\u0131m Bankas\u0131 A.\u015e."
     },
     {
-        "bank_code": "0152",
+        "bank_code": "00152",
         "bic": "DEYATRIS",
         "country_code": "TR",
         "name": "Destek Yat\u0131r\u0131m Bankas\u0131 A.\u015e.",
         "primary": true,
         "short_name": "Destek Yat\u0131r\u0131m Bankas\u0131 A.\u015e."
     },
     {
```

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/__init__.py` & `schwifty-2024.4.0/schwifty/checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/czech_republic.py` & `schwifty-2024.4.0/schwifty/checksum/czech_republic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/estonia.py` & `schwifty-2024.4.0/schwifty/checksum/estonia.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/france.py` & `schwifty-2024.4.0/schwifty/checksum/france.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/germany.py` & `schwifty-2024.4.0/schwifty/checksum/germany.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Checksum algorithms for German Bank institutes.
 
 A description of the algorithms can be found on the website of the Bundesbank
 
 https://www.bundesbank.de/resource/blob/603320/16a80c739bbbae592ca575905975c2d0/mL/pruefzifferberechnungsmethoden-data.pdf
 """
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from itertools import cycle
 from typing import ClassVar
 
 from schwifty import checksum
```

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/iceland.py` & `schwifty-2024.4.0/schwifty/checksum/iceland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/italy.py` & `schwifty-2024.4.0/schwifty/checksum/italy.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/netherlands.py` & `schwifty-2024.4.0/schwifty/checksum/netherlands.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/norway.py` & `schwifty-2024.4.0/schwifty/checksum/norway.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         total: int = 0
         for n, c in zip(weights, value):
             total += n * int(c)
 
         check_digit = 11 - (total % 11)
         if check_digit == 10:
             raise InvalidAccountCode("Check digit does not compute: Invalid account code.")
-        return str(check_digit % 10)
+        return str(check_digit % 11)
```

### Comparing `schwifty-2024.1.1.post0/schwifty/checksum/spain.py` & `schwifty-2024.4.0/schwifty/checksum/spain.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/iban_registry/README.md` & `schwifty-2024.4.0/schwifty/iban_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/iban_registry/generated.json` & `schwifty-2024.4.0/schwifty/iban_registry/generated.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/schwifty/iban_registry/overwrite.json` & `schwifty-2024.4.0/schwifty/iban_registry/overwrite.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859154929577465%*

 * *Differences: {'delete': "['DK']"}*

```diff
@@ -331,26 +331,14 @@
             ],
             "national_checksum_digits": [
                 21,
                 23
             ]
         }
     },
-    "DK": {
-        "positions": {
-            "account_code": [
-                4,
-                13
-            ],
-            "national_checksum_digits": [
-                13,
-                14
-            ]
-        }
-    },
     "DZ": {
         "bban_length": 22,
         "bban_spec": "22!n",
         "iban_length": 26,
         "iban_spec": "DZ2!n22!n",
         "in_sepa_zone": false,
         "positions": {
```

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_at.py` & `schwifty-2024.4.0/scripts/get_bank_registry_at.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_be.py` & `schwifty-2024.4.0/scripts/get_bank_registry_be.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_ch.py` & `schwifty-2024.4.0/scripts/get_bank_registry_ch.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_cz.py` & `schwifty-2024.4.0/scripts/get_bank_registry_cz.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas
 
 
 URL = "https://www.cnb.cz/cs/platebni-styk/.galleries/ucty_kody_bank/download/kody_bank_CR.csv"
 
 
 def process():
-    datas = pandas.read_csv(URL, encoding="latin1", delimiter=";", dtype="str")
+    datas = pandas.read_csv(URL, encoding="utf-8", delimiter=";", dtype="str")
     datas = datas.dropna(how="all")
     datas.fillna("", inplace=True)
 
     registry = []
     for row in datas.itertuples(index=False):
         registry.append(
             {
```

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_de.py` & `schwifty-2024.4.0/scripts/get_bank_registry_de.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_es.py` & `schwifty-2024.4.0/scripts/get_bank_registry_es.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_fi.py` & `schwifty-2024.4.0/scripts/get_bank_registry_fi.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_hr.py` & `schwifty-2024.4.0/scripts/get_bank_registry_hr.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_hu.py` & `schwifty-2024.4.0/scripts/get_bank_registry_hu.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_it.py` & `schwifty-2024.4.0/scripts/get_bank_registry_it.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_lt.py` & `schwifty-2024.4.0/scripts/get_bank_registry_lt.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_lv.py` & `schwifty-2024.4.0/scripts/get_bank_registry_lv.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_nl.py` & `schwifty-2024.4.0/scripts/get_bank_registry_nl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_no.py` & `schwifty-2024.4.0/scripts/get_bank_registry_no.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_pl.py` & `schwifty-2024.4.0/scripts/get_bank_registry_pl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_ro.py` & `schwifty-2024.4.0/scripts/get_bank_registry_ro.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_se.py` & `schwifty-2024.4.0/scripts/get_bank_registry_se.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_si.py` & `schwifty-2024.4.0/scripts/get_bank_registry_si.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_sk.py` & `schwifty-2024.4.0/scripts/get_bank_registry_sk.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_bank_registry_ua.py` & `schwifty-2024.4.0/scripts/get_bank_registry_ua.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/scripts/get_iban_registry.py` & `schwifty-2024.4.0/scripts/get_iban_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/tests/test_bic.py` & `schwifty-2024.4.0/tests/test_bic.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         ("IT", "01030", "PASCITMM"),  # curated
         ("LV", "RIKO", "RIKOLV2XXXX"),
         ("MC", "30003", "SOGEMCM1"),
         ("NL", "ADYB", "ADYBNL2A"),
         ("PL", "10100055", "NBPLPLPWXXX"),
         ("PL", "10900004", "WBKPPLPPXXX"),
         ("RO", "BPOS", "BPOSROBU"),
-        ("SA", "NBPA", "NBPASARI"),
         ("SE", "500", "ESSESESS"),
         ("SI", "01050", "BSLJSI2XFNB"),
         ("SK", "0900", "GIBASKBX"),
     ],
 )
 def test_bic_from_bank_code(country: str, bank_code: str, bic: str) -> None:
     assert BIC.from_bank_code(country, bank_code).compact == bic
@@ -185,14 +184,15 @@
                 "BNPAFRPPIFO",
             ],
         ),
         ("DE", "43060967", ["GENODEM1GLS"]),
         ("HU", "107", ["CIBHHUHB"]),
         ("HR", "2485003", ["CROAHR2X"]),
         ("LV", "RIKO", ["RIKOLV2XXXX"]),
+        ("ME", "907", ["CBCGMEPG"]),
         ("NL", "ADYB", ["ADYBNL2A"]),
         ("PL", "10100055", ["NBPLPLPWXXX"]),
         ("RO", "BPOS", ["BPOSROBU"]),
         ("SE", "500", ["ESSESESS"]),
         ("SI", "01050", ["BSLJSI2XFNB"]),
         ("SK", "0900", ["GIBASKBX"]),
     ],
```

### Comparing `schwifty-2024.1.1.post0/tests/test_checksum.py` & `schwifty-2024.4.0/tests/test_checksum.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,7 +101,11 @@
 
 def test_belgium_checksum_checksum_edge_case() -> None:
     assert algorithms["BE:default"].validate(["050", "0000177"], "97") is True
 
 
 def test_netherlands_checksum() -> None:
     assert algorithms["NL:default"].validate(["0417164300"], "") is True
+
+
+def test_norway_checksum_checksum_edge_case() -> None:
+    assert algorithms["NO:default"].validate(["6042", "143964"], "0") is True
```

### Comparing `schwifty-2024.1.1.post0/tests/test_iban.py` & `schwifty-2024.4.0/tests/test_iban.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,15 @@
         (("BE", "050", "123"), "BE66050000012343"),
         (("BE", "050", "123456"), "BE45050012345689"),
         (("BE", "539", "0075470"), "BE68539007547034"),
         (("BE", "050", "177"), "BE54050000017797"),
         (("DE", "43060967", "7000534100"), "DE42430609677000534100"),
         (("DE", "51230800", "2622196545"), "DE61512308002622196545"),
         (("DE", "20690500", "9027378"), "DE37206905000009027378"),
+        (("DK", "0040", "0440116243"), "DK5000400440116243"),
         (("FR", "2004101005", "0500013M026"), "FR1420041010050500013M02606"),
         (("GB", "NWBK", "31926819", "601613"), "GB29NWBK60161331926819"),
         (("GB", "NWBK", "31926819"), "GB66NWBK00000031926819"),
         (("GB", "NWBK601613", "31926819"), "GB29NWBK60161331926819"),
         (("IT", "0538703601", "000000198036"), "IT18T0538703601000000198036"),
         (("IT", "0538703601", "000000198060"), "IT57V0538703601000000198060"),
         (("IT", "0538703601", "000000198072"), "IT40Z0538703601000000198072"),
```

### Comparing `schwifty-2024.1.1.post0/LICENSE` & `schwifty-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/README.rst` & `schwifty-2024.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.1.1.post0/hatch.toml` & `schwifty-2024.4.0/hatch.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [envs.default]
 dependencies = [
-  "freezegun==1.2.*",
+  "freezegun==1.4.*",
   "pytest-cov==4.1.*",
-  "pytest==7.3.*",
+  "pytest==8.1.*",
 ]
 features = [
   "pydantic",
 ]
 
 [envs.default.scripts]
 cov-test = "pytest --cov=schwifty {args:tests schwifty}"
 test = "cov-test --no-cov"
 
 [envs.lint]
 extra-dependencies = [
-  "ruff==0.1.*",
-  "black==23.12.*",
-  "mypy==1.8.*",
+  "ruff==0.3.*",
+  "mypy==1.9.*",
   "doc8==1.1.*",
   "pygments==2.16.*",
 ]
 
 [envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:schwifty tests}"
 style = [
-  "black --check --diff {args:.}",
-  "ruff {args:.}",
+  "ruff format --check --diff {args:.}",
+  "ruff check {args:.}",
 ]
 fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
+  "ruff format {args:.}",
+  "ruff check --fix {args:.}",
 ]
 docs = "doc8 docs/source"
```

### Comparing `schwifty-2024.1.1.post0/pyproject.toml` & `schwifty-2024.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "Martin Domke", email = "mail@martindomke.net" },
 ]
 dependencies = [
-    "importlib_resources; python_version <= '3.8'",
+    "importlib_resources>=5.10; python_version <= '3.11'",
     "iso3166",
     "pycountry",
 ]
 
 [project.optional-dependencies]
 pydantic = [
     "pydantic>=2.0"
@@ -45,58 +45,54 @@
 source = "vcs"
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "schwifty",
 ]
 
-[tool.black]
-line-length = 100
-
 [tool.pytest.pytest.ini_options]
 addopts = """
   --pyargs schwifty
   --doctest-modules
   --junit-xml test-results.xml
   --cov-report xml
   --cov-report term-missing
 """
 console_output_style = "progress"
 doctest_optionflags = "ALLOW_UNICODE IGNORE_EXCEPTION_DETAIL"
 
 [tool.ruff]
 target-version = "py38"
 line-length = 100
+
+[tool.ruff.lint]
 select = ["A", "B", "C", "C4", "E", "F", "I", "N", "PT", "Q", "RUF", "S", "SIM", "T10", "UP", "W", "YTT"]
 fixable = ["RUF100", "I001"]
 ignore = [
     "S101",   # Allow usage of asserts
     "A001",   # Allow shadowing bultins 
     "A003",   # Allow shadowing bultins on classes
 ]
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 "scripts/get_*_registry*.py" = [
     "S113",   # Allow requests call without timeout
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 lines-after-imports = 2
 order-by-type = false
 
-[tool.isort]
-profile = "black"
-force_alphabetical_sort_within_sections = true
-force_single_line = true
-lines_after_imports = 2
-line_length = 100
-
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["ulid"]
 
 [tool.doc8]
 max-line-length = 100
+
+[tool.mypy]
+exclude = ["docs"]
```

### Comparing `schwifty-2024.1.1.post0/PKG-INFO` & `schwifty-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: schwifty
-Version: 2024.1.1.post0
+Version: 2024.4.0
 Project-URL: Changelog, https://github.com/mdomke/schwifty/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://schwifty.readthedocs.io/en/latest/
 Project-URL: Homepage, http://github.com/mdomke/schwifty
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.8
-Requires-Dist: importlib-resources; python_version <= '3.8'
+Requires-Dist: importlib-resources>=5.10; python_version <= '3.11'
 Requires-Dist: iso3166
 Requires-Dist: pycountry
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0; extra == 'pydantic'
 Description-Content-Type: text/x-rst
 
 .. image:: https://img.shields.io/pypi/v/schwifty.svg?style=flat-square
```

