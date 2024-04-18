# Comparing `tmp/paraphase-3.1.0.tar.gz` & `tmp/paraphase-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paraphase-3.1.0.tar", last modified: Wed Apr 17 03:53:44 2024, max compression
+gzip compressed data, was "paraphase-3.1.1.tar", last modified: Thu Apr 18 18:31:39 2024, max compression
```

## Comparing `paraphase-3.1.0.tar` & `paraphase-3.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.762002 paraphase-3.1.0/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-3.1.0/LICENSE
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7393 2024-04-17 03:53:44.761011 paraphase-3.1.0/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7063 2024-04-16 20:57:56.000000 paraphase-3.1.0/README.md
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:43.958038 paraphase-3.1.0/paraphase/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2024-04-15 22:17:28.000000 paraphase-3.1.0/paraphase/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2024-01-11 16:37:31.000000 paraphase-3.1.0/paraphase/__main__.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.051052 paraphase-3.1.0/paraphase/data/
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.114039 paraphase-3.1.0/paraphase/data/19/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5390 2024-04-15 21:55:28.000000 paraphase-3.1.0/paraphase/data/19/config.yaml
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.145036 paraphase-3.1.0/paraphase/data/19/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/rccx/cyp21_diff_sites.txt
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1053 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/sex_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.176028 paraphase-3.1.0/paraphase/data/19/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/19/smn1/known_haplotypes.json
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.272028 paraphase-3.1.0/paraphase/data/38/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    40934 2024-04-12 16:48:47.000000 paraphase-3.1.0/paraphase/data/38/config.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    43629 2024-02-02 18:15:30.000000 paraphase-3.1.0/paraphase/data/38/fusion_genes.json
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.296027 paraphase-3.1.0/paraphase/data/38/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/rccx/cyp21_diff_sites.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1104 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/sex_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.343024 paraphase-3.1.0/paraphase/data/38/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/data/38/smn1/known_haplotypes.json
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      194 2024-02-21 18:17:36.000000 paraphase-3.1.0/paraphase/data/genes.yaml
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.616006 paraphase-3.1.0/paraphase/genes/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      425 2024-02-14 20:04:22.000000 paraphase-3.1.0/paraphase/genes/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2937 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/cfc1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1531 2024-02-15 03:52:32.000000 paraphase-3.1.0/paraphase/genes/cfhclust.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     8240 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/f8_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5788 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/hba_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7553 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/ikbkg_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4936 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/ncf1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5659 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/neb_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    17211 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/opn1lw_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     4353 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/pms2_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    19955 2024-03-26 20:30:17.000000 paraphase-3.1.0/paraphase/genes/rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25155 2024-01-11 16:37:50.000000 paraphase-3.1.0/paraphase/genes/smn1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5707 2024-01-11 16:37:51.000000 paraphase-3.1.0/paraphase/genes/strc_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2791 2024-01-11 16:37:51.000000 paraphase-3.1.0/paraphase/genome_depth.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    48834 2024-01-11 16:37:32.000000 paraphase-3.1.0/paraphase/haplotype_assembler.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30906 2024-04-15 22:34:32.000000 paraphase-3.1.0/paraphase/paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    86230 2024-04-16 03:39:23.000000 paraphase-3.1.0/paraphase/phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    45486 2024-04-09 23:05:47.000000 paraphase-3.1.0/paraphase/prepare_bam_and_vcf.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.034037 paraphase-3.1.0/paraphase.egg-info/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7393 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1456 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/SOURCES.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/dependency_links.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/entry_points.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/requires.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2024-04-17 03:53:42.000000 paraphase-3.1.0/paraphase.egg-info/top_level.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2024-04-17 03:53:44.762015 paraphase-3.1.0/setup.cfg
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2024-01-11 16:37:32.000000 paraphase-3.1.0/setup.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-17 03:53:44.749003 paraphase-3.1.0/tests/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1110 2024-03-26 20:30:19.000000 paraphase-3.1.0/tests/test_f8_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2024-01-11 16:37:32.000000 paraphase-3.1.0/tests/test_haplotype_assembler.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4712 2024-01-11 16:37:51.000000 paraphase-3.1.0/tests/test_opn1lw_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2024-01-11 16:37:32.000000 paraphase-3.1.0/tests/test_paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    12210 2024-04-16 01:39:44.000000 paraphase-3.1.0/tests/test_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4372 2024-04-15 16:41:24.000000 paraphase-3.1.0/tests/test_prepare_bam_and_vcf.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2024-01-11 16:37:33.000000 paraphase-3.1.0/tests/test_rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     7844 2024-01-11 16:37:51.000000 paraphase-3.1.0/tests/test_smn1_phaser.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.439480 paraphase-3.1.1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-3.1.1/LICENSE
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7775 2024-04-18 18:31:39.438477 paraphase-3.1.1/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7445 2024-04-17 21:51:32.000000 paraphase-3.1.1/README.md
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.250492 paraphase-3.1.1/paraphase/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2024-04-18 16:11:09.000000 paraphase-3.1.1/paraphase/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2024-01-11 16:37:31.000000 paraphase-3.1.1/paraphase/__main__.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.284506 paraphase-3.1.1/paraphase/data/
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.309497 paraphase-3.1.1/paraphase/data/19/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5390 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/data/19/config.yaml
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/19/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.313488 paraphase-3.1.1/paraphase/data/19/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/19/rccx/cyp21_diff_sites.txt
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1053 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/19/sex_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.328482 paraphase-3.1.1/paraphase/data/19/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/19/smn1/known_haplotypes.json
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.346489 paraphase-3.1.1/paraphase/data/38/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    40934 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/data/38/config.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    43629 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/data/38/fusion_genes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/38/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.367477 paraphase-3.1.1/paraphase/data/38/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/38/rccx/cyp21_diff_sites.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1104 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/38/sex_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.370497 paraphase-3.1.1/paraphase/data/38/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/data/38/smn1/known_haplotypes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      194 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/data/genes.yaml
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.414474 paraphase-3.1.1/paraphase/genes/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      425 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2937 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/cfc1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1815 2024-04-17 21:31:47.000000 paraphase-3.1.1/paraphase/genes/cfhclust.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     8240 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/f8_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5788 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/genes/hba_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7553 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/genes/ikbkg_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4936 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/ncf1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5659 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/neb_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    17211 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/opn1lw_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     4353 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/pms2_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    19955 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/genes/rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25155 2024-01-11 16:37:50.000000 paraphase-3.1.1/paraphase/genes/smn1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5707 2024-01-11 16:37:51.000000 paraphase-3.1.1/paraphase/genes/strc_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     3493 2024-04-18 16:47:33.000000 paraphase-3.1.1/paraphase/genome_depth.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    48834 2024-01-11 16:37:32.000000 paraphase-3.1.1/paraphase/haplotype_assembler.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30907 2024-04-18 16:31:46.000000 paraphase-3.1.1/paraphase/paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    86230 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    45486 2024-04-17 16:00:35.000000 paraphase-3.1.1/paraphase/prepare_bam_and_vcf.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.281499 paraphase-3.1.1/paraphase.egg-info/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7775 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1456 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/entry_points.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/requires.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2024-04-18 18:31:38.000000 paraphase-3.1.1/paraphase.egg-info/top_level.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2024-04-18 18:31:39.439486 paraphase-3.1.1/setup.cfg
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2024-01-11 16:37:32.000000 paraphase-3.1.1/setup.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2024-04-18 18:31:39.435484 paraphase-3.1.1/tests/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1110 2024-04-17 16:00:35.000000 paraphase-3.1.1/tests/test_f8_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2024-01-11 16:37:32.000000 paraphase-3.1.1/tests/test_haplotype_assembler.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4712 2024-01-11 16:37:51.000000 paraphase-3.1.1/tests/test_opn1lw_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2024-01-11 16:37:32.000000 paraphase-3.1.1/tests/test_paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    12210 2024-04-17 16:00:35.000000 paraphase-3.1.1/tests/test_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4372 2024-04-17 16:00:36.000000 paraphase-3.1.1/tests/test_prepare_bam_and_vcf.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2024-01-11 16:37:33.000000 paraphase-3.1.1/tests/test_rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     7844 2024-01-11 16:37:51.000000 paraphase-3.1.1/tests/test_smn1_phaser.py
```

### Comparing `paraphase-3.1.0/LICENSE` & `paraphase-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/PKG-INFO` & `paraphase-3.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 3.1.0
+Version: 3.1.1
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,16 @@
 <h1 align="center">Paraphase</h1>
 
 <h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
-Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
+Paraphase takes all reads from a gene family, realigns to one representative gene of the family and then phases them into haplotypes. This approach bypasses the error-prone process of aligning reads to multiple similar regions and allows us to examine all copies of genes in a gene family. This gene-family-centered approach allows Paraphase to perform well when there is a copy number difference between an individual and the reference, as is often the case in segmental duplications.
+Futhermore, this approach also streamlines sequence comparisons between genes within the same family, making it straightforward to conduct analyses such as identifying non-allelic gene conversions.  
 
 Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
@@ -88,15 +89,15 @@
 - `-r`: Path to the reference genome fasta file
 
 Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
 - `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the header of the input BAM. 
 - `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
 - `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
```

### Comparing `paraphase-3.1.0/README.md` & `paraphase-3.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 <h1 align="center">Paraphase</h1>
 
 <h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
-Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
+Paraphase takes all reads from a gene family, realigns to one representative gene of the family and then phases them into haplotypes. This approach bypasses the error-prone process of aligning reads to multiple similar regions and allows us to examine all copies of genes in a gene family. This gene-family-centered approach allows Paraphase to perform well when there is a copy number difference between an individual and the reference, as is often the case in segmental duplications.
+Futhermore, this approach also streamlines sequence comparisons between genes within the same family, making it straightforward to conduct analyses such as identifying non-allelic gene conversions.  
 
 Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
@@ -77,15 +78,15 @@
 - `-r`: Path to the reference genome fasta file
 
 Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
 - `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the header of the input BAM. 
 - `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
 - `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
```

### Comparing `paraphase-3.1.0/paraphase/data/19/config.yaml` & `paraphase-3.1.1/paraphase/data/19/config.yaml`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/19/genome_region.bed` & `paraphase-3.1.1/paraphase/data/19/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/19/sex_region.bed` & `paraphase-3.1.1/paraphase/data/19/sex_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/19/smn1/known_haplotypes.json` & `paraphase-3.1.1/paraphase/data/19/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/38/config.yaml` & `paraphase-3.1.1/paraphase/data/38/config.yaml`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/38/fusion_genes.json` & `paraphase-3.1.1/paraphase/data/38/fusion_genes.json`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/38/genome_region.bed` & `paraphase-3.1.1/paraphase/data/38/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/38/sex_region.bed` & `paraphase-3.1.1/paraphase/data/38/sex_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/data/38/smn1/known_haplotypes.json` & `paraphase-3.1.1/paraphase/data/38/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/cfc1_phaser.py` & `paraphase-3.1.1/paraphase/genes/cfc1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/cfhclust.py` & `paraphase-3.1.1/paraphase/genes/cfhclust.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,20 +15,28 @@
     ):
         Phaser.__init__(self, sample_id, outdir)
         self.cfh = cfh
         self.cfhr3 = cfhr3
 
     def call(self):
         haps = {}
-        haps.update(self.cfh["final_haplotypes"])
-        haps.update(self.cfhr3["final_haplotypes"])
         fusions = {}
-        fusions.update(self.cfh["fusions_called"])
-        fusions.update(self.cfhr3["fusions_called"])
         total_cn = None
+        if (
+            self.cfh["final_haplotypes"] is not None
+            and self.cfhr3["final_haplotypes"] is not None
+        ):
+            haps.update(self.cfh["final_haplotypes"])
+            haps.update(self.cfhr3["final_haplotypes"])
+        if (
+            self.cfh["fusions_called"] is not None
+            and self.cfhr3["fusions_called"] is not None
+        ):
+            fusions.update(self.cfh["fusions_called"])
+            fusions.update(self.cfhr3["fusions_called"])
         if self.cfh["total_cn"] is not None and self.cfhr3["total_cn"] is not None:
             total_cn = min(self.cfh["total_cn"], self.cfhr3["total_cn"])
             if (
                 fusions != {}
                 and len(self.cfh["final_haplotypes"]) >= 2
                 and len(self.cfhr3["final_haplotypes"]) >= 2
             ):
```

### Comparing `paraphase-3.1.0/paraphase/genes/f8_phaser.py` & `paraphase-3.1.1/paraphase/genes/f8_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/hba_phaser.py` & `paraphase-3.1.1/paraphase/genes/hba_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/ikbkg_phaser.py` & `paraphase-3.1.1/paraphase/genes/ikbkg_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/ncf1_phaser.py` & `paraphase-3.1.1/paraphase/genes/ncf1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/neb_phaser.py` & `paraphase-3.1.1/paraphase/genes/neb_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/opn1lw_phaser.py` & `paraphase-3.1.1/paraphase/genes/opn1lw_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/pms2_phaser.py` & `paraphase-3.1.1/paraphase/genes/pms2_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/rccx_phaser.py` & `paraphase-3.1.1/paraphase/genes/rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/smn1_phaser.py` & `paraphase-3.1.1/paraphase/genes/smn1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/genes/strc_phaser.py` & `paraphase-3.1.1/paraphase/genes/strc_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/haplotype_assembler.py` & `paraphase-3.1.1/paraphase/haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/paraphase.py` & `paraphase-3.1.1/paraphase/paraphase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     VcfGenerater,
     TwoGeneVcfGenerater,
 )
 import paraphase
 from paraphase import genes
 from .phaser import Phaser
 
-logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.INFO)
 
 
 class Paraphase:
     def __init__(self):
         self.samtools = None
         self.minimap2 = None
 
@@ -586,15 +586,15 @@
             help="Output directory",
             required=True,
         )
         parser.add_argument(
             "-p",
             "--prefix",
             help="Prefix of output files for a single sample. Used with -b.\n"
-            + "If not provided, prefix will be extracted from the name of the input BAM.\n",
+            + "If not provided, prefix will be extracted from the header of the input BAM.\n",
             required=False,
         )
         parser.add_argument(
             "-g",
             "--gene",
             help="Optionally specify which gene(s) to run (separated by comma).\n"
             + "Will run all genes if not specified.\n"
```

### Comparing `paraphase-3.1.0/paraphase/phaser.py` & `paraphase-3.1.1/paraphase/phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase/prepare_bam_and_vcf.py` & `paraphase-3.1.1/paraphase/prepare_bam_and_vcf.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/paraphase.egg-info/PKG-INFO` & `paraphase-3.1.1/paraphase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 3.1.0
+Version: 3.1.1
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,16 @@
 <h1 align="center">Paraphase</h1>
 
 <h3 align="center">HiFi-based caller for highly similar paralogous genes</h3>
 
 Many medically relevant genes fall into 'dark' regions where variant calling is limited due to high sequence homology with paralogs or pseudogenes. Paraphase is a Python tool that takes HiFi aligned BAMs as input (whole-genome or enrichment), phases haplotypes for genes of the same family, determines copy numbers and makes phased variant calls. 
 
 ![Paraphase diagram](docs/figures/paraphase_diagram.png)
-Paraphase takes all reads from a gene family, realigns to just the gene of interest and then phases them into haplotypes. This solves the problem of alignment difficulty due to sequence homology and allows us to examine all copies of genes in a gene family and call copy number changes and other variants.
+Paraphase takes all reads from a gene family, realigns to one representative gene of the family and then phases them into haplotypes. This approach bypasses the error-prone process of aligning reads to multiple similar regions and allows us to examine all copies of genes in a gene family. This gene-family-centered approach allows Paraphase to perform well when there is a copy number difference between an individual and the reference, as is often the case in segmental duplications.
+Futhermore, this approach also streamlines sequence comparisons between genes within the same family, making it straightforward to conduct analyses such as identifying non-allelic gene conversions.  
 
 Paraphase supports 160 segmental duplication [regions](docs/regions.md) in GRCh38. Among these, there are 11 medically relevant regions that are also supported in GRCh37/hg19:
 - SMN1/SMN2 (spinal muscular atrophy)
 - RCCX module
   - CYP21A2 (21-Hydroxylase-Deficient Congenital Adrenal Hyperplasia)
   - TNXB (Ehlers-Danlos syndrome)
   - C4A/C4B (relevant in autoimmune diseases)
@@ -88,15 +89,15 @@
 - `-r`: Path to the reference genome fasta file
 
 Please note that the input BAM should be one that's aligned to the ENTIRE reference genome (either GRCh38 or GRCh37/hg19), and this reference should NOT include ALT contigs. The fasta file of this reference genome should be provided to Paraphase with `-r`. Recommendations on reference genomes to use are documented [here](https://github.com/PacificBiosciences/reference_genomes).
 
 Optional parameters:
 - `-g`: Region(s) to analyze, separated by comma. All supported [regions](docs/regions.md) will be analyzed if not specified. Please use region name, i.e. first column in the doc.
 - `-t`: Number of threads.
-- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the name of the input BAM. 
+- `-p`: Prefix of output files when the input is a single sample, i.e. use with `-b`. If not provided, prefix will be extracted from the header of the input BAM. 
 - `--genome`: Genome reference build. Default is `38`. If `37` or `19` is specified, Paraphase will run the analysis for GRCh37 or hg19, respectively (note that only 11 medically relevant [regions](docs/regions.md) are supported now for GRCh37/hg19).
 - `--gene1only`: If specified, variants calls will be made against the main gene only for SMN1, PMS2, STRC, NCF1 and IKBKG, see more information [here](docs/vcf.md).
 - `--novcf`: If specified, no VCF files will be produced.
 - `--samtools`: path to samtools. If the paths to samtools or minimap2 are not already in the PATH environment variable, they can be provided through the `--samtools` and `--minimap2` parameters.
 - `--minimap2`: path to minimap2
 
 ## Interpreting the output
```

### Comparing `paraphase-3.1.0/paraphase.egg-info/SOURCES.txt` & `paraphase-3.1.1/paraphase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/setup.py` & `paraphase-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_f8_phaser.py` & `paraphase-3.1.1/tests/test_f8_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_haplotype_assembler.py` & `paraphase-3.1.1/tests/test_haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_opn1lw_phaser.py` & `paraphase-3.1.1/tests/test_opn1lw_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_paraphase.py` & `paraphase-3.1.1/tests/test_paraphase.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_phaser.py` & `paraphase-3.1.1/tests/test_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_prepare_bam_and_vcf.py` & `paraphase-3.1.1/tests/test_prepare_bam_and_vcf.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_rccx_phaser.py` & `paraphase-3.1.1/tests/test_rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-3.1.0/tests/test_smn1_phaser.py` & `paraphase-3.1.1/tests/test_smn1_phaser.py`

 * *Files identical despite different names*

