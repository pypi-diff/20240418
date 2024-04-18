# Comparing `tmp/dsharp_opac-1.1.7.tar.gz` & `tmp/dsharp_opac-1.1.8rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsharp_opac-1.1.7.tar", last modified: Fri May  5 08:54:31 2023, max compression
+gzip compressed data, was "dsharp_opac-1.1.8rc0.tar", last modified: Thu Apr 18 14:26:51 2024, max compression
```

## Comparing `dsharp_opac-1.1.7.tar` & `dsharp_opac-1.1.8rc0.tar`

### file list

```diff
@@ -1,145 +1,109 @@
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.638718 dsharp_opac-1.1.7/
--rw-r--r--   0 birnstiel   (501) staff       (20)    35140 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/LICENSE
--rw-r--r--   0 birnstiel   (501) staff       (20)      224 2019-02-18 12:53:11.000000 dsharp_opac-1.1.7/MANIFEST.in
--rw-r--r--   0 birnstiel   (501) staff       (20)     2537 2023-05-05 08:54:31.638575 dsharp_opac-1.1.7/PKG-INFO
--rw-r--r--   0 birnstiel   (501) staff       (20)     2220 2019-03-15 10:56:48.000000 dsharp_opac-1.1.7/README.md
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.589046 dsharp_opac-1.1.7/dsharp_opac/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2133 2023-05-05 08:53:32.000000 dsharp_opac-1.1.7/dsharp_opac/__init__.py
--rw-r--r--   0 birnstiel   (501) staff       (20)    11792 2020-11-19 08:45:02.000000 dsharp_opac-1.1.7/dsharp_opac/bhmie_fortran.f90
--rw-r--r--   0 birnstiel   (501) staff       (20)     6931 2019-02-20 21:12:46.000000 dsharp_opac-1.1.7/dsharp_opac/bhmie_python.py
--rw-r--r--   0 birnstiel   (501) staff       (20)      414 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/calldraine.f90
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.602161 dsharp_opac-1.1.7/dsharp_opac/data/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2184 2019-07-30 08:34:28.000000 dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     2093 2019-07-30 08:45:33.000000 dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1301 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/data/andrews2009.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   803630 2019-02-04 20:34:40.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   803274 2019-02-19 21:16:44.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_extrapol.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   853812 2019-02-05 22:29:36.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_smooth.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   843960 2023-03-22 13:18:30.000000 dsharp_opac-1.1.7/dsharp_opac/data/diana.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   803316 2019-02-04 20:37:06.000000 dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   853427 2019-02-05 22:37:57.000000 dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities_smooth.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)     2260 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)    15708 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/dsharp_opac/data/kataoka_mix.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)  2143594 2021-08-04 15:23:22.000000 dsharp_opac-1.1.7/dsharp_opac/data/ricci_compact.npz
--rwxr-xr-x   0 birnstiel   (501) staff       (20)    98010 2023-04-18 14:25:51.000000 dsharp_opac-1.1.7/dsharp_opac/dsharp_opac.py
--rw-r--r--   0 birnstiel   (501) staff       (20)    25142 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/fit_module.f90
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.586661 dsharp_opac-1.1.7/dsharp_opac/optical_constants/
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.609582 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/
--rw-r--r--   0 birnstiel   (501) staff       (20)      144 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)    22981 2022-02-15 11:30:37.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpaD03_0.01
--rw-r--r--   0 birnstiel   (501) staff       (20)    22981 2022-02-15 11:30:39.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpaD03_0.10
--rw-r--r--   0 birnstiel   (501) staff       (20)    22804 2022-02-15 11:30:40.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpeD03_0.01
--rw-r--r--   0 birnstiel   (501) staff       (20)    22804 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpeD03_0.10
--rw-r--r--   0 birnstiel   (501) staff       (20)    49590 2022-02-15 11:30:35.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_silD03
--rw-r--r--   0 birnstiel   (501) staff       (20)    62740 2022-02-15 11:30:34.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/eps_Sil
--rw-r--r--   0 birnstiel   (501) staff       (20)    70053 2022-02-15 11:30:36.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/eps_suvSil
--rw-r--r--   0 birnstiel   (501) staff       (20)      827 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.609836 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/
--rw-r--r--   0 birnstiel   (501) staff       (20)        6 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/.gitignore
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.611465 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/ironk.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1058 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/links.json
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olivinenewk.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olmg60k.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olmg70k.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/organicsk.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg100k.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg60k.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg70k.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/troilitek.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/watericek.lnk
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.612390 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/iron.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      599 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/links.json
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/olivine.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/organics.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/orthopyr.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/troilite.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/waterice.lnk
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.614068 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/
--rw-r--r--   0 birnstiel   (501) staff       (20)       45 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)     3796 2022-07-22 11:56:08.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel1000.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     3588 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel400.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     3536 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel600.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     3692 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel800.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.615168 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/
--rw-r--r--   0 birnstiel   (501) staff       (20)    75634 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   132169 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   132175 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/silicate.dat
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.618605 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/
--rw-r--r--   0 birnstiel   (501) staff       (20)      580 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)      568 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1331 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1078 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1656 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1168 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1705 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1060 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      666 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)      505 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2009 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      887 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/make_lnk.py
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.618907 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/
--rw-r--r--   0 birnstiel   (501) staff       (20)       23 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      215 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.619202 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/
--rw-r--r--   0 birnstiel   (501) staff       (20)       15 2019-03-14 19:07:11.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      137 2019-03-14 19:07:12.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.621999 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/
--rw-r--r--   0 birnstiel   (501) staff       (20)      882 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)  2351704 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
--rw-r--r--   0 birnstiel   (501) staff       (20)    10382 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
--rw-r--r--   0 birnstiel   (501) staff       (20)      509 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.625852 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/
--rw-r--r--   0 birnstiel   (501) staff       (20)       24 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)    16514 2022-02-15 11:30:33.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/IOP_2008_ASCIItable.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)      122 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/links.json
--rw-r--r--   0 birnstiel   (501) staff       (20)    13224 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)     4525 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.626903 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/
--rw-r--r--   0 birnstiel   (501) staff       (20)     1052 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)     1097 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      812 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      731 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      818 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      750 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)   915276 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.590459 dsharp_opac-1.1.7/dsharp_opac.egg-info/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2537 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/PKG-INFO
--rw-r--r--   0 birnstiel   (501) staff       (20)     5739 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/SOURCES.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)        1 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/dependency_links.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)        1 2022-02-09 13:20:56.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/not-zip-safe
--rw-r--r--   0 birnstiel   (501) staff       (20)       38 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/requires.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)       12 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/top_level.txt
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.638287 dsharp_opac-1.1.7/notebooks/
--rw-r--r--   0 birnstiel   (501) staff       (20)    18210 2023-01-27 08:30:29.000000 dsharp_opac-1.1.7/notebooks/AppendixB.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     4632 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure1.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     1719 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/notebooks/Figure2.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     2339 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure3.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     3963 2022-06-13 07:04:00.000000 dsharp_opac-1.1.7/notebooks/Figure4.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     6886 2023-01-27 08:24:20.000000 dsharp_opac-1.1.7/notebooks/Figure56.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     4105 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure7.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    11439 2023-03-30 09:03:24.000000 dsharp_opac-1.1.7/notebooks/Figure8.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     3854 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure9.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     5933 2020-12-01 11:32:58.000000 dsharp_opac-1.1.7/notebooks/aux_functions.py
--rw-r--r--   0 birnstiel   (501) staff       (20)     5917 2020-06-08 18:32:14.000000 dsharp_opac-1.1.7/notebooks/dsharp_porosity.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)      394 2018-12-10 20:04:26.000000 dsharp_opac-1.1.7/notebooks/header.py
--rw-r--r--   0 birnstiel   (501) staff       (20)     1514 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/notebooks/index.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    12688 2019-02-20 20:53:26.000000 dsharp_opac-1.1.7/notebooks/opac_widget.py
--rw-r--r--   0 birnstiel   (501) staff       (20)  1816292 2019-07-26 10:44:58.000000 dsharp_opac-1.1.7/notebooks/opacity_examples.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)   609690 2019-02-20 19:44:13.000000 dsharp_opac-1.1.7/notebooks/opacity_package_tests.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    50797 2020-03-31 07:16:03.000000 dsharp_opac-1.1.7/notebooks/polarization_fraction.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     8660 2020-03-31 07:18:07.000000 dsharp_opac-1.1.7/notebooks/porosity.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     7303 2023-03-30 09:07:49.000000 dsharp_opac-1.1.7/notebooks/rosseland_mean_opacities.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     6503 2019-07-26 10:45:36.000000 dsharp_opac-1.1.7/notebooks/scattering_phase_functions.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    16618 2020-06-08 18:18:17.000000 dsharp_opac-1.1.7/notebooks/smoothed_opacities.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)       38 2023-05-05 08:54:31.638769 dsharp_opac-1.1.7/setup.cfg
--rw-r--r--   0 birnstiel   (501) staff       (20)     2049 2020-11-11 14:25:34.000000 dsharp_opac-1.1.7/setup.py
+-rw-r--r--   0        0        0      191 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/.gitignore
+-rw-r--r--   0        0        0    35140 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/LICENSE
+-rw-r--r--   0        0        0      224 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/MANIFEST.in
+-rw-r--r--   0        0        0     2190 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/README.md
+-rw-r--r--   0        0        0        8 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/apt.txt
+-rw-r--r--   0        0        0     2190 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/__init__.py
+-rw-r--r--   0        0        0    11792 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/bhmie_fortran.f90
+-rw-r--r--   0        0        0     6931 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/bhmie_python.py
+-rw-r--r--   0        0        0      414 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/calldraine.f90
+-rw-r--r--   0        0        0     2184 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
+-rw-r--r--   0        0        0     2093 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
+-rw-r--r--   0        0        0     1301 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/andrews2009.dat
+-rw-r--r--   0        0        0   803630 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities.npz
+-rw-r--r--   0        0        0   803274 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities_extrapol.npz
+-rw-r--r--   0        0        0   853812 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities_smooth.npz
+-rw-r--r--   0        0        0   803316 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/icefree_opacities.npz
+-rw-r--r--   0        0        0   853427 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/icefree_opacities_smooth.npz
+-rw-r--r--   0        0        0     2260 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
+-rw-r--r--   0        0        0    15708 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/kataoka_mix.lnk
+-rw-r--r--   0        0        0      444 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/meson.build
+-rw-r--r--   0        0        0  2143594 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/data/ricci_compact.npz
+-rwxr-xr-x   0        0        0    99617 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/dsharp_opac.py
+-rw-r--r--   0        0        0    25142 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/fit_module.f90
+-rw-r--r--   0        0        0     1182 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/meson.build
+-rw-r--r--   0        0        0      144 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/draine/.gitignore
+-rw-r--r--   0        0        0      827 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/draine/links.json
+-rw-r--r--   0        0        0      130 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/draine/meson.build
+-rw-r--r--   0        0        0        6 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/.gitignore
+-rw-r--r--   0        0        0       27 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/meson.build
+-rw-r--r--   0        0        0     1058 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/new/links.json
+-rw-r--r--   0        0        0      135 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/new/meson.build
+-rw-r--r--   0        0        0      599 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/old/links.json
+-rw-r--r--   0        0        0      135 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/old/meson.build
+-rw-r--r--   0        0        0       45 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/jaeger/.gitignore
+-rw-r--r--   0        0        0      425 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/jaeger/links.json
+-rw-r--r--   0        0        0      130 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/jaeger/meson.build
+-rw-r--r--   0        0        0    75634 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
+-rw-r--r--   0        0        0   132169 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
+-rw-r--r--   0        0        0      180 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/meson.build
+-rw-r--r--   0        0        0   132175 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/silicate.dat
+-rw-r--r--   0        0        0      199 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/meson.build
+-rw-r--r--   0        0        0      580 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
+-rw-r--r--   0        0        0      568 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
+-rw-r--r--   0        0        0     1331 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
+-rw-r--r--   0        0        0     1078 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
+-rw-r--r--   0        0        0     1656 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
+-rw-r--r--   0        0        0     1168 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
+-rw-r--r--   0        0        0     1705 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
+-rw-r--r--   0        0        0     1060 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
+-rw-r--r--   0        0        0      666 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
+-rw-r--r--   0        0        0      505 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
+-rw-r--r--   0        0        0     2009 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
+-rw-r--r--   0        0        0     1425 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
+-rw-r--r--   0        0        0     7500 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
+-rw-r--r--   0        0        0      887 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/make_lnk.py
+-rw-r--r--   0        0        0      593 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/meson.build
+-rw-r--r--   0        0        0       23 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/preibisch/.gitignore
+-rw-r--r--   0        0        0      215 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/preibisch/links.json
+-rw-r--r--   0        0        0      133 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/preibisch/meson.build
+-rw-r--r--   0        0        0       15 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/segelstein_water/.gitignore
+-rw-r--r--   0        0        0      137 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/segelstein_water/links.json
+-rw-r--r--   0        0        0      140 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/segelstein_water/meson.build
+-rw-r--r--   0        0        0      882 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
+-rw-r--r--   0        0        0  2351704 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
+-rw-r--r--   0        0        0    10382 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
+-rw-r--r--   0        0        0      509 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
+-rw-r--r--   0        0        0      208 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/meson.build
+-rw-r--r--   0        0        0       24 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/.gitignore
+-rw-r--r--   0        0        0      122 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/links.json
+-rw-r--r--   0        0        0      186 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/meson.build
+-rw-r--r--   0        0        0    13224 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/warren_1984.txt
+-rw-r--r--   0        0        0     4525 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
+-rw-r--r--   0        0        0      276 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/meson.build
+-rw-r--r--   0        0        0     1052 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
+-rw-r--r--   0        0        0     1097 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
+-rw-r--r--   0        0        0      812 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
+-rw-r--r--   0        0        0      731 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
+-rw-r--r--   0        0        0      818 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
+-rw-r--r--   0        0        0      750 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
+-rw-r--r--   0        0        0   915276 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
+-rw-r--r--   0        0        0      539 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/meson.build
+-rw-r--r--   0        0        0    18210 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/AppendixB.ipynb
+-rw-r--r--   0        0        0     4632 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure1.ipynb
+-rw-r--r--   0        0        0     1719 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure2.ipynb
+-rw-r--r--   0        0        0     2339 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure3.ipynb
+-rw-r--r--   0        0        0     3963 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure4.ipynb
+-rw-r--r--   0        0        0     6886 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure56.ipynb
+-rw-r--r--   0        0        0     4105 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure7.ipynb
+-rw-r--r--   0        0        0    11407 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure8.ipynb
+-rw-r--r--   0        0        0     3854 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/Figure9.ipynb
+-rw-r--r--   0        0        0     5933 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/aux_functions.py
+-rw-r--r--   0        0        0     5917 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/dsharp_porosity.ipynb
+-rw-r--r--   0        0        0      394 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/header.py
+-rw-r--r--   0        0        0     1514 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/index.ipynb
+-rw-r--r--   0        0        0    12688 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/opac_widget.py
+-rw-r--r--   0        0        0  1816292 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/opacity_examples.ipynb
+-rw-r--r--   0        0        0   609690 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/opacity_package_tests.ipynb
+-rw-r--r--   0        0        0    50797 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/polarization_fraction.ipynb
+-rw-r--r--   0        0        0     8660 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/porosity.ipynb
+-rw-r--r--   0        0        0     6503 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/scattering_phase_functions.ipynb
+-rw-r--r--   0        0        0    16618 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/notebooks/smoothed_opacities.ipynb
+-rw-r--r--   0        0        0      528 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-18 14:26:38.000000 dsharp_opac-1.1.8rc0/requirements.txt
+-rw-r--r--   0        0        0    43129 2024-04-18 14:26:51.857686 dsharp_opac-1.1.8rc0/PKG-INFO
```

### Comparing `dsharp_opac-1.1.7/LICENSE` & `dsharp_opac-1.1.8rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/PKG-INFO` & `dsharp_opac-1.1.8rc0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: dsharp_opac
-Version: 1.1.7
-Summary: python routines to calculate mie opacities
-Home-page: https://github.com/birnstiel/dsharp_opac
-Author: Til Birnstiel & DSHARP collaboration
-Author-email: til.birnstiel@lmu.de
-License: GPLv3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b04c8f86251749ac92361c6431103a08)](https://app.codacy.com/app/birnstiel/dsharp_opac?utm_source=github.com&utm_medium=referral&utm_content=birnstiel/dsharp_opac&utm_campaign=Badge_Grade_Dashboard)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/b31911d281014b5197cb4ef1acb32cf3)](https://app.codacy.com/gh/birnstiel/dsharp_opac/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![DOI](https://zenodo.org/badge/137751482.svg)](https://zenodo.org/badge/latestdoi/137751482)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/birnstiel/dsharp_opac/master?filepath=notebooks%2Findex.ipynb)
 
 # DSHARP Mie-Opacity Library
 
 This repository contains a module to carry out Mie opacity calculations based on
 a range of astrophysically relevant optical datasets and to calculate the
```

### Comparing `dsharp_opac-1.1.7/dsharp_opac/__init__.py` & `dsharp_opac-1.1.8rc0/dsharp_opac/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from importlib import metadata as _md
 from .bhmie_python import bhmie_python
 try:
     from .bhmie_fortran import bhmie_fortran
 except ImportError:
     print('fortran mie routines unavailable')
 
-__version__ = '1.1.7'
+__version__ = _md.version("dsharp_opac")
 
 from .dsharp_opac import \
     progress_bar, \
     diel_const, \
     diel_from_lnk_file, \
     diel_henning, \
     diel_jaeger98, \
```

### Comparing `dsharp_opac-1.1.7/dsharp_opac/bhmie_fortran.f90` & `dsharp_opac-1.1.8rc0/dsharp_opac/bhmie_fortran.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/bhmie_python.py` & `dsharp_opac-1.1.8rc0/dsharp_opac/bhmie_python.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/andrews2009.dat` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/andrews2009.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_extrapol.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities_extrapol.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_smooth.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/default_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/icefree_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities_smooth.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/icefree_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/kataoka_mix.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/kataoka_mix.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/data/ricci_compact.npz` & `dsharp_opac-1.1.8rc0/dsharp_opac/data/ricci_compact.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/dsharp_opac.py` & `dsharp_opac-1.1.8rc0/dsharp_opac/dsharp_opac.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   the functions `diel_*.nk` return the optical properties
 """
 from __future__ import print_function
 import numpy as np
 import os
 import sys
 import warnings
-import pkg_resources
+import importlib
 import astropy.constants as const
 from pathlib import Path
 from scipy.interpolate import interp2d, RegularGridInterpolator
 
 au = const.au.cgs.value
 M_sun = const.M_sun.cgs.value
 k_b = const.k_B.cgs.value
@@ -37,24 +37,26 @@
 
 try:
     from .bhmie_fortran import bhmie_fortran
     bhmie_function = bhmie_fortran
     bhmie_type = 'fortran'
 
 except ImportError:
-    warnings.warn('could not import compiled mie code - mie calculation will be slow')
+    warnings.warn(
+        'could not import compiled mie code - mie calculation will be slow')
     from .bhmie_python import bhmie_python_wrapper
     from .bhmie_python import bhmie_type as bt
     bhmie_type = bt
     bhmie_function = bhmie_python_wrapper
 
     try:
         from numba import njit  # noqa
     except ImportError:
-        warnings.warn('numba not available, opacity calculation will be very slow')
+        warnings.warn(
+            'numba not available, opacity calculation will be very slow')
 
 try:
     import pymiecoated
 
     def bhmie_pymiecoated(x, nk, n_angles):
         """
         Wrapper to the Mie code of `pymiecoated`
@@ -105,15 +107,16 @@
     pass
 
 try:
     from .fit_module import fit_module
     distribution = fit_module.fit_function18_test
 except ImportError:
     def distribution(*args, **kwargs):
-        raise ImportError('fortran size distribution code unavailable! Apparently it was not installed with f2py')
+        raise ImportError(
+            'fortran size distribution code unavailable! Apparently it was not installed with f2py')
 
 
 def progress_bar(perc, text=''):
     """
     Displays a progress bar.
 
     This is a very simple progress bar which displays the given
@@ -153,15 +156,15 @@
         file name of data file
 
     Output
     ------
     str : absolute path to data file
 
     """
-    return pkg_resources.resource_filename(__name__, os.path.join(base, fname))
+    return importlib.resources.files(__name__).joinpath(base).joinpath(fname)
 
 
 def download(packagedir):
     """
     Downloads the optical constants files. It works by getting the data from
     a json file `links.json` in `packagedir`.
     """
@@ -176,15 +179,16 @@
 
     with open(os.path.join(packagedir, 'links.json')) as f:
         data = json.load(f)
         for material, link in data.items():
 
             filename = link.split('/')[-1]
 
-            print('material: {}, downloading {}: ... '.format(material, filename), end='')
+            print('material: {}, downloading {}: ... '.format(
+                material, filename), end='')
             try:
                 urlretrieve(link, filename=os.path.join(packagedir, filename))
                 print('Done!')
             except Exception as ex:
                 print('Failed!')
                 raise ex
 
@@ -232,15 +236,16 @@
         self._lmax = lam[-1]
         self._has_negative_n = np.any(n <= 0)
         self.print_reference()
 
     def print_reference(self, appendix=''):
         """Prints the citation request, appends appendix"""
         if self.reference is not None:
-            print('Please cite {} when using these optical constants'.format(self.reference) + appendix)
+            print('Please cite {} when using these optical constants'.format(
+                self.reference) + appendix)
 
     def nk(self, lam):
         """
         Return the optical properties interpolated at wavelength lam
 
         Arguments:
         ----------
@@ -253,27 +258,30 @@
         n : float
         :    real part of optical property
 
         k : float
         :    imaginary part of optical property
         """
         if np.array(lam, ndmin=1).min() < self._lmin or np.array(lam, ndmin=1).max() > self._lmax:
-            raise NameError('{}: wavelength {:g} outside data-range [{:g},{:g}]'.format(type(self).__name__, lam, self._lmin, self._lmax))
+            raise NameError('{}: wavelength {:g} outside data-range [{:g},{:g}]'.format(
+                type(self).__name__, lam, self._lmin, self._lmax))
 
         log_interp = True
         if self._has_negative_n:
             # estimate if log interpolation is ok to do
             n = np.interp(lam, self._l, self._n)
             if n < 0:
                 log_interp = False
 
         if log_interp:
-            result = 10.**np.interp(np.log10(lam), self._ll, self._ln), 10.**np.interp(np.log10(lam), self._ll, self._lk)
+            result = 10.**np.interp(np.log10(lam), self._ll,
+                                    self._ln), 10.**np.interp(np.log10(lam), self._ll, self._lk)
         else:
-            result = np.interp(lam, self._l, self._n), 10.**np.interp(np.log10(lam), self._ll, self._lk)
+            result = np.interp(
+                lam, self._l, self._n), 10.**np.interp(np.log10(lam), self._ll, self._lk)
 
         return result
 
     def extrapolate_constants_up(self, lmin, lmax, n=10, kind='second'):
         """
         Extend the data by log-extrapolation to longer wavelengths. Will start
         fitting for extrapolation at lmin and then extend the data up to lmax.
@@ -296,15 +304,16 @@
             - 'first', 'second': do a first or second order extrapolation
         """
         #
         # extrapolate
         #
         self.extrapol = True
         if self._has_negative_n:
-            warnings.warn('Extrapolation for negative n values can cause issues')
+            warnings.warn(
+                'Extrapolation for negative n values can cause issues')
 
         l_ext = np.logspace(np.log10(self._l[-1]), np.log10(lmax), n)[1:]
         from scipy.optimize import curve_fit
 
         if kind == 'constant':
             n_ext = self._n[-1] * np.ones_like(l_ext)
             k_ext = self._k[-1] * np.ones_like(l_ext)
@@ -330,20 +339,22 @@
             raise ValueError('unknown extrapolation method')
 
         if kind != 'constant':
             i_min = abs(self._l - lmin).argmin()
             #
             # extrapolate n
             #
-            res = curve_fit(f, np.log10(self._l[i_min:]), np.log10(self._n[i_min:]), p0_n)
+            res = curve_fit(f, np.log10(
+                self._l[i_min:]), np.log10(self._n[i_min:]), p0_n)
             n_ext = 10.**f(np.log10(l_ext), *res[0])
             #
             # extrapolate k
             #
-            res = curve_fit(f, np.log10(self._l[i_min:]), np.log10(self._k[i_min:]), p0_k)
+            res = curve_fit(f, np.log10(
+                self._l[i_min:]), np.log10(self._k[i_min:]), p0_k)
             k_ext = 10.**f(np.log10(l_ext), *res[0])
 
         # update attributes
 
         self._l = np.append(self._l, l_ext)
         self._n = np.append(self._n, n_ext)
         self._k = np.append(self._k, k_ext)
@@ -360,15 +371,16 @@
         fitting for extrapolation at lmax and then extend the data down to lmin.
         """
         #
         # extrapolate
         #
         self.extrapol = True
         if self._has_negative_n:
-            warnings.warn('Extrapolation for negative n values can cause issues')
+            warnings.warn(
+                'Extrapolation for negative n values can cause issues')
 
         l_ext = np.logspace(np.log10(lmin), np.log10(self._l[0]), n)[:-1]
         from scipy.optimize import curve_fit
 
         if kind == 'constant':
             n_ext = self._n[0] * np.ones_like(l_ext)
             k_ext = self._k[0] * np.ones_like(l_ext)
@@ -394,20 +406,22 @@
             raise ValueError('`kind` must be `first` or `second`')
 
         if kind != 'constant':
             i_max = abs(self._l - lmax).argmin()
             #
             # extrapolate n
             #
-            res = curve_fit(f, np.log10(self._l[:i_max]), np.log10(self._n[:i_max]), p0_n)
+            res = curve_fit(f, np.log10(
+                self._l[:i_max]), np.log10(self._n[:i_max]), p0_n)
             n_ext = 10.**f(np.log10(l_ext), *res[0])
             #
             # extrapolate k
             #
-            res = curve_fit(f, np.log10(self._l[:i_max]), np.log10(self._k[:i_max]), p0_k)
+            res = curve_fit(f, np.log10(
+                self._l[:i_max]), np.log10(self._k[:i_max]), p0_k)
             k_ext = 10.**f(np.log10(l_ext), *res[0])
 
         # update attributes
 
         self._l = np.append(l_ext, self._l)
         self._n = np.append(n_ext, self._n)
         self._k = np.append(k_ext, self._k)
@@ -507,15 +521,16 @@
         self.material_str = species[0].upper() + species[1:] + ' (Henning)'
 
         if iron_abundance not in ['normal', 'low', 'high']:
             raise NameError('unknown iron abundance')
         if species not in ['iron', 'olivine', 'organics', 'orthopyroxene', 'troilite', 'waterice']:
             raise NameError('unknown abundance species')
         if (iron_abundance != 'normal') and ((not new) or (species not in ['olivine', 'orthopyroxene'])):
-            raise NameError('low & high iron only available for new olivine and new orthopyroxene')
+            raise NameError(
+                'low & high iron only available for new olivine and new orthopyroxene')
         #
         # set the file name
         #
         if species in ['iron', 'organics', 'troilite', 'waterice']:
             fname = species + new * 'k'
         elif species == 'olivine':
             if iron_abundance == 'normal':
@@ -547,16 +562,18 @@
             'organics': 1.5 * refractory + 1.0 * (not refractory),
             'troilitek': 4.83,
             'troilite': 4.83,
             'watericek': 0.92,
             'waterice': 0.92
         }
         self.rho = densities[fname]
-        self.datafile = get_datafile(os.path.join('henning', 'new' * new + 'old' * (not new), fname + '.lnk'), base='optical_constants')
-        self.reference = 'Henning & Stognienko (1996)' + (not new) * ', Pollack et al. (1994)'
+        self.datafile = get_datafile(os.path.join(
+            'henning', 'new' * new + 'old' * (not new), fname + '.lnk'), base='optical_constants')
+        self.reference = 'Henning & Stognienko (1996)' + \
+            (not new) * ', Pollack et al. (1994)'
         if not os.path.isfile(self.datafile):
             self.download()
         #
         # read data
         #
         print('Reading opacities from %s' % fname)
         data = np.loadtxt(self.datafile)
@@ -572,15 +589,16 @@
         self._lmin = self._l.min()
         self._lmax = self._l.max()
         self.print_reference()
 
     @classmethod
     def download(self):
         for i in ['old', 'new']:
-            path = get_datafile(os.path.join('henning', i), base='optical_constants')
+            path = get_datafile(os.path.join('henning', i),
+                                base='optical_constants')
             download(path)
 
 
 class diel_jaeger98(diel_const):
     """
     Returns the dielectric constants for the various carbonaceous dust optical
     constants from:
@@ -607,19 +625,21 @@
         #
         # set the path and do some safety checks
         #
         temps = [400, 600, 800, 1000]
         rhos = [1.435, 1.670, 1.843, 1.988]
         if T not in temps:
             raise AssertionError("invalid temperature, use {}".format(temps))
-        self.material_str = 'Carbonaceous dust, T={} C (Jaeger et al. 1998)'.format(T)
+        self.material_str = 'Carbonaceous dust, T={} C (Jaeger et al. 1998)'.format(
+            T)
         self.rho = rhos[temps.index(T)]
 
         fname = 'cel{}.lnk'.format(T)
-        self.datafile = get_datafile(os.path.join('jaeger', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'jaeger', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
         #
         # read data
         #
         print('Reading opacities from %s' % fname)
         data = np.loadtxt(self.datafile)
@@ -657,15 +677,16 @@
         #
         # set the path and do some safety checks
         #
         self.material_str = 'Liquid water, T=25 C (Segelstein 1981)'
         self.rho = 0.997
 
         fname = 'Segelstein.csv'
-        self.datafile = get_datafile(os.path.join('segelstein_water', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'segelstein_water', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
         #
         # read data
         #
         print('Reading opacities from %s' % fname)
         with open(self.datafile) as f:
@@ -727,23 +748,26 @@
         """
         #
         # set the path and do some safety checks
         #
         species = species.lower()
         options = ['dirty ice', 'amorphous carbon']
         if species not in options:
-            raise AssertionError("unknown species, use one of {}".format(options))
-        self.material_str = '{}, (Preibisch et al. 1993)'.format(species.capitalize())
+            raise AssertionError(
+                "unknown species, use one of {}".format(options))
+        self.material_str = '{}, (Preibisch et al. 1993)'.format(
+            species.capitalize())
 
         if species == 'dirty ice':
             fname = 'diiceneu.lnk'
         elif species == 'amorphous carbon':
             fname = 'acneu.lnk'
 
-        self.datafile = get_datafile(os.path.join('preibisch', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'preibisch', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
         #
         # read data
         #
         print('Reading opacities from %s' % fname)
         data = np.loadtxt(self.datafile)
@@ -793,22 +817,26 @@
         """
         Overwrite the initialization of the parent class
         """
         #
         # set the path and do some safety checks
         #
         species = species.lower()
-        options = ['water ice', 'troilite', 'organics', 'olivine', 'iron', 'orthopyroxene']
+        options = ['water ice', 'troilite', 'organics',
+                   'olivine', 'iron', 'orthopyroxene']
         if species not in options:
-            raise AssertionError("unknown species, use one of {}".format(options))
-        self.material_str = '{}, (Pollack et al. 1994)'.format(species.capitalize())
+            raise AssertionError(
+                "unknown species, use one of {}".format(options))
+        self.material_str = '{}, (Pollack et al. 1994)'.format(
+            species.capitalize())
 
         fname = 'P94-{}.lnk'.format(species.replace(' ', ''))
 
-        self.datafile = get_datafile(os.path.join('pollack1994', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'pollack1994', fname), base='optical_constants')
         #
         # read data
         #
         print('Reading opacities from %s' % fname)
         data = np.loadtxt(self.datafile)
         #
         # assign wavelength and optical constants
@@ -858,37 +886,43 @@
 
     def __init__(self, species, **kwargs):
         """
         Overwrite the initialization of the parent class
         """
         options = ['astrosilicates', 'graphite']
         if species.lower() not in options:
-            raise AssertionError('unknown species, use one of {}'.format(options))
+            raise AssertionError(
+                'unknown species, use one of {}'.format(options))
         #
         # open file, read header and data
         #
         if species.lower() == 'astrosilicates':
             self.material_str = 'Astronomical Silicates (Draine 2003)'
             fname = 'callindex.out_silD03'
             self.rho = 3.3  # laor & draine 93
 
         elif species.lower() == 'graphite':
             if 'parallel' not in kwargs:
-                raise AssertionError('bool keyword \'parallel\' needed for graphite grains')
+                raise AssertionError(
+                    'bool keyword \'parallel\' needed for graphite grains')
             if 'a' not in kwargs:
-                raise AssertionError('str keyword \'a\' needed for graphite grains')
+                raise AssertionError(
+                    'str keyword \'a\' needed for graphite grains')
             parallel = kwargs.pop('parallel')
             a = kwargs.pop('a')
-            self.material_str = 'Graphite, {}, a={} mu (Laor & Draine 1993)'.format(parallel * 'pa' + (not parallel) * 'pe', a)
-            fname = 'callindex.out_C{}D03_{}'.format('pa' * parallel + 'pe' * (not parallel), a)
+            self.material_str = 'Graphite, {}, a={} mu (Laor & Draine 1993)'.format(
+                parallel * 'pa' + (not parallel) * 'pe', a)
+            fname = 'callindex.out_C{}D03_{}'.format(
+                'pa' * parallel + 'pe' * (not parallel), a)
             self.rho = 2.26  # laor & draine 93
 
         # download file if needed
 
-        self.datafile = get_datafile(os.path.join('draine', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'draine', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
 
         # read from file
 
         with open(self.datafile) as f:
             self.headerinfo = [f.readline() for i in range(5)]
@@ -924,15 +958,16 @@
         """
         Overwrite the initialization of the parent class
         """
         #
         # open file, read header and data
         #
         self.material_str = 'Astronomical Silicates (Weingartner & Draine 2001)'
-        self.datafile = get_datafile(os.path.join('draine', 'eps_suvSil'), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'draine', 'eps_suvSil'), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
         f = open(self.datafile)
         self.headerinfo = [f.readline() for i in range(9)]
         data = np.loadtxt(f)
         #
         # assign wavelength and optical constants
@@ -966,15 +1001,16 @@
         """
         Overwrite the initialization of the parent class
         """
         #
         # open file, read header and data
         #
         self.material_str = 'Astronomical Silicates (Draine & Lee 1984)'
-        self.datafile = get_datafile(os.path.join('draine', 'eps_Sil'), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'draine', 'eps_Sil'), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(os.path.dirname(self.datafile))
         with open(self.datafile) as f:
             self.headerinfo = [f.readline() for i in range(6)]
             data = np.loadtxt(f)
         #
         # assign wavelength and optical constants
@@ -1054,20 +1090,24 @@
         Overwrite the initialization of the parent class
         """
         #
         # open files, read data
         #
         directory = os.path.join('optical_constants', 'zubko+1996')
 
-        self.material_str = 'Carbonaceous Grains (Zubko et al. 1996, {})'.format(sample)
+        self.material_str = 'Carbonaceous Grains (Zubko et al. 1996, {})'.format(
+            sample)
         self.datafile = directory
 
-        E = np.loadtxt(get_datafile(os.path.join('zubko_E_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
-        n = np.loadtxt(get_datafile(os.path.join('zubko_n_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
-        k = np.loadtxt(get_datafile(os.path.join('zubko_k_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
+        E = np.loadtxt(get_datafile(os.path.join(
+            'zubko_E_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
+        n = np.loadtxt(get_datafile(os.path.join(
+            'zubko_n_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
+        k = np.loadtxt(get_datafile(os.path.join(
+            'zubko_k_{}.txt'.format(sample)), base=self.datafile))[-1::-1]
         l = 0.00012398419292004205 / E  # E = h*c/lambda in CGS # noqa
         #
         # assign wavelength and optical constants
         #
         self._l = l
         self._n = n
         self._k = k
@@ -1100,15 +1140,16 @@
         #
         self.material_str = 'Water Ice (Warren 1984)'
         self.reference = 'Warren (1984)'
         #
         # set the file name
         #
         fname = 'warren_1984.txt'
-        self.datafile = get_datafile(os.path.join('warren', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'warren', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(self.datafile)
         #
         # read data and assign wavelength and optical constants
         #
         data = np.loadtxt(self.datafile)
         self._l = data[:, 0] * 1e-4
@@ -1146,15 +1187,16 @@
         #
         self.material_str = 'Water Ice (Warren & Brandt 2008)'
         self.reference = 'Warren & Brandt (2008)'
         #
         # set the file name
         #
         fname = 'IOP_2008_ASCIItable.dat'
-        self.datafile = get_datafile(os.path.join('warren', fname), base='optical_constants')
+        self.datafile = get_datafile(os.path.join(
+            'warren', fname), base='optical_constants')
         if not os.path.isfile(self.datafile):
             download(self.datafile)
         #
         # read data and assign wavelength and optical constants
         #
         data = np.loadtxt(self.datafile)
         self._l = data[:, 0] * 1e-4
@@ -1205,28 +1247,31 @@
     def __init__(self, species, extrapol=False, lmin=None, lmax=10.0):
         """
         Overwrite the initialization of the parent class
         """
         #
         # set the path and do some safety checks
         #
-        self.material_str = ('Ricci et al. 2010, ' + species).replace('ice', 'water ice')
+        self.material_str = ('Ricci et al. 2010, ' +
+                             species).replace('ice', 'water ice')
         self.extrapol = extrapol
         #
         # set the file name
         #
         if species == 'silicate':
             fname = 'silicate.dat'
         elif species == 'ice':
             fname = 'H2Oice_Warren.dat'
         elif species == 'carbon':
             fname = 'aC_ACH2_Zubko.dat'
         else:
-            raise NameError('%s got unknown species: %s' % (type(self).__name__, species))
-        self.datafile = get_datafile(os.path.join('luca', fname), base='optical_constants')
+            raise NameError('%s got unknown species: %s' %
+                            (type(self).__name__, species))
+        self.datafile = get_datafile(os.path.join(
+            'luca', fname), base='optical_constants')
         #
         # read data and assign wavelength and optical constants
         #
         f = open(self.datafile)
         self.headerinfo = [f.readline() for i in range(2)]
         data = np.loadtxt(f)
         l = data[:, 0] * 1e-4  # noqa
@@ -1245,21 +1290,23 @@
             def fct(x, a, b, c):
                 return a + b * x + c * x**2
 
             i_min = abs(l - 1e-1).argmin()
             #
             # extrapolate n
             #
-            res = curve_fit(fct, np.log10(l[i_min:]), np.log10(n[i_min:]), [np.log10(n[-1]), 1, 0])
+            res = curve_fit(fct, np.log10(l[i_min:]), np.log10(
+                n[i_min:]), [np.log10(n[-1]), 1, 0])
             ne = 10.**fct(np.log10(le), *res[0])
             n = np.append(n, ne)
             #
             # extrapolate k
             #
-            res = curve_fit(fct, np.log10(l[i_min:]), np.log10(k[i_min:]), [np.log10(k[-1]), 1, 0])
+            res = curve_fit(fct, np.log10(l[i_min:]), np.log10(
+                k[i_min:]), [np.log10(k[-1]), 1, 0])
             ke = 10.**fct(np.log10(le), *res[0])
             k = np.append(k, ke)
             l = np.append(l, le)  # noqa
             #
             # LOWER EXTRAPOLATION: constant
             #
             if lmin is not None:
@@ -1317,15 +1364,16 @@
 
         extrapol : bool
             whether or not to extrapolate constants beyond there defined interval
         """
         if rule.lower() not in ['bruggeman', 'maxwell-garnett']:
             raise NameError('Unknown mixing rule: %s' % rule)
         if rule.lower() == 'maxwell-garnett':
-            print('using Maxwell-Garnett mixing: first component should be host material (= matrix)')
+            print(
+                'using Maxwell-Garnett mixing: first component should be host material (= matrix)')
             if constants[0].material_str is not None:
                 print('    matrix = {}'.format(constants[0].material_str))
 
         self.material_str = '%s-Mix of %i species' % (rule, len(constants))
         self.constants = constants
         self.abundances = abundances
         self.rule = rule
@@ -1528,15 +1576,16 @@
     """
     sigma_d = sigma_g * d2g
 
     m = 4 * np.pi / 3 * rho_s * a**3  # mass grid
 
     # create the size distribution
 
-    res = distribution(11 / 6., T, alpha, sigma_g, sigma_d, rho_s, m, a, M_star, r, v_frag)
+    res = distribution(11 / 6., T, alpha, sigma_g, sigma_d,
+                       rho_s, m, a, M_star, r, v_frag)
     fit = res[0]
 
     return fit
 
 
 def get_B11S_fit(T, a, r=au, sigma_g=200., d2g=0.01, rho_s=1.6686, M_star=M_sun,
                  v_frag=100., alpha=4e-4, mu=2.3, stokes_regime=False):
@@ -1615,15 +1664,16 @@
     if stokes_regime:
         a_fr_St1 = (9. * St_f * sigma_g * mfp / (2. * np.pi * rho_s))**0.5
         a_frag = np.minimum(a_frag, a_fr_St1)
 
     # if no fragmentation is happening: return NANs
 
     if np.isnan(a_frag) or a_frag > a[-1] or a_frag < a[0]:
-        warnings.warn('Fragmentation size outside grid, no size distribution returned')
+        warnings.warn(
+            'Fragmentation size outside grid, no size distribution returned')
         return np.zeros_like(a) * np.nan, np.nan
 
     # calculate settling size
 
     a_set = 2. * sigma_g / (np.pi * rho_s) * alpha
     if stokes_regime:
         a_set_St1 = (9. * alpha * sigma_g * mfp / (2. * np.pi * rho_s))**0.5
@@ -1652,15 +1702,16 @@
         elif a_regime <= a_12:
             slope = slopes[i_s, 1]
         else:
             slope = slopes[i_s, 2]
 
         # make the size distribution
 
-        sigma_d[ia_prev:ia_next + 1] = sigma_d[ia_prev] * (a[ia_prev:ia_next + 1] / a[ia_prev])**(slope - 1)
+        sigma_d[ia_prev:ia_next + 1] = sigma_d[ia_prev] * \
+            (a[ia_prev:ia_next + 1] / a[ia_prev])**(slope - 1)
 
         ia_prev = ia_next
 
     # implement a floor value for all particles above fragmentation velocity
 
     sigma_d[a >= a_frag] = 1e-100
 
@@ -1740,15 +1791,16 @@
     -------
     kappa_abs,kappa_sca : array
         the opacity at each wavelength averaged over the size
         distribution and normalized per 1 g of dust.
     """
     if (q_abs is None or q_sca is None) and (kappa_abs is None or kappa_sca is None) \
             and (diel_const is None):
-        raise AssertionError('Either (diel_const) or (q_abs, q_sca) or (k_abs, k_sca) needed as input')
+        raise AssertionError(
+            'Either (diel_const) or (q_abs, q_sca) or (k_abs, k_sca) needed as input')
     #
     # some basic conversions
     #
     m = 4. * np.pi / 3. * rho_s * a**3
     sig = n * m * a
     sig = sig / sum(sig)
     #
@@ -1870,15 +1922,16 @@
 
     # issue a warning for large size parameters
 
     xmax = 2. * np.pi / LAM.min() * A.max()
     xstop = xmax + 4. * xmax**.333333 + 2.0
     nmx = (xstop.max() + 15).max()
     if nmx > 2e5 and extrapolate_large_grains is False:
-        warnings.warn('large size parameter: nmx={} - this can take long'.format(nmx))
+        warnings.warn(
+            'large size parameter: nmx={} - this can take long'.format(nmx))
     #
     # the wave length loop
     #
     for ilam, lam in enumerate(LAM):
         #
         # display progress
         #
@@ -1914,29 +1967,31 @@
                 return x + 4. * x**0.33333 + 2.0 - NMXX
             x_max = fsolve(f, NMXX)  # /30.
             X_cut = [x_max]
         #
         # loop through the sizes that converge
         #
         for ia, x in enumerate(X_cut):
-            S1, S2, _, Qabs, Qsca, _, gsca = bhmie_function(x, complex(n, k), nang)
+            S1, S2, _, Qabs, Qsca, _, gsca = bhmie_function(
+                x, complex(n, k), nang)
             q_abs[ia, ilam] = Qabs
             q_sca[ia, ilam] = Qsca
             g_sca[ia, ilam] = gsca.real
             s_1[ia, ilam, :] = S1
             s_2[ia, ilam, :] = S2
         #
         # extrapolate for large grains
         #
         q_abs[ia + 1:, ilam] = q_abs[ia, ilam]
         q_sca[ia + 1:, ilam] = q_sca[ia, ilam]
 
         # Laor & Draine 1993, Eq. 8
 
-        g_sca[ia + 1:, ilam] = 0.3 * X[ia + 1:]**2 / (1 + 0.3 * X[ia + 1:]**2)  # g_sca[ia, ilam]
+        g_sca[ia + 1:, ilam] = 0.3 * X[ia + 1:]**2 / \
+            (1 + 0.3 * X[ia + 1:]**2)  # g_sca[ia, ilam]
 
     package = {
         'q_abs': q_abs,
         'q_sca': q_sca,
         'g': g_sca,
         'S1': s_1,
         'S2': s_2,
@@ -2020,23 +2075,25 @@
     error_max = 0.0
     if theta is not None and k_sca is not None:
         n_theta = len(theta)
         mu = np.cos(theta * np.pi / 180.)
         dmu = np.diff(mu)
         for ia in range(len(m)):
             for ilam in range(len(lam)):
-                zav = 0.5 * (zscat[ia, ilam, 1:n_theta, 0] + zscat[ia, ilam, 0:n_theta - 1, 0])
+                zav = 0.5 * (zscat[ia, ilam, 1:n_theta, 0] +
+                             zscat[ia, ilam, 0:n_theta - 1, 0])
                 dum = -0.5 * zav * dmu
                 integral = dum.sum() * 4 * np.pi
                 kscat_from_z11[ia, ilam] = integral
                 err = abs(integral / k_sca[ia, ilam] - 1.0)
                 error_max = max(err, error_max)
 
     if error_max > error_tolerance:
-        warnings.warn('Maximum error of {:.2g}%: above error tolerance'.format(error_max * 100))
+        warnings.warn(
+            'Maximum error of {:.2g}%: above error tolerance'.format(error_max * 100))
 
     return {'zscat': zscat, 'kscat_from_z11': kscat_from_z11, 'error_max': error_max}
 
 
 def make_opacity_dict(lam, a, k_abs, k_sca, g_sca, rho_s, zscat=None):
     """
     To mimick the behavior of the `makedustopac.py` code by Kees Dullemond:
@@ -2088,21 +2145,25 @@
     ---------
 
     path : str
         path where to store the file, defaults to current directory
     """
 
     if 'a' not in opac_dict:
-        raise AssertionError('opacity dictionary needs to contain particle size array \'a\'')
+        raise AssertionError(
+            'opacity dictionary needs to contain particle size array \'a\'')
     if 'lam' not in opac_dict:
-        raise AssertionError('opacity dictionary needs to contain wave length array \'lam\'')
+        raise AssertionError(
+            'opacity dictionary needs to contain wave length array \'lam\'')
     if 'k_abs' not in opac_dict:
-        raise AssertionError('opacity dictionary needs to contain absortpion opacity array \'k_abs\'')
+        raise AssertionError(
+            'opacity dictionary needs to contain absortpion opacity array \'k_abs\'')
     if 'k_sca' not in opac_dict:
-        raise AssertionError('opacity dictionary needs to contain scattering opacity array \'k_sca\'')
+        raise AssertionError(
+            'opacity dictionary needs to contain scattering opacity array \'k_sca\'')
 
     # build a dict that contains only the data we need
 
     dictionary = {}
     dictionary['a'] = opac_dict['a']
     dictionary['lam'] = opac_dict['lam']
     dictionary['k_abs'] = opac_dict['k_abs']
@@ -2234,15 +2295,16 @@
         # if a_grain is given: interpolate (log-log in kappa, log-lin in g)
 
         lam = opac_dict['lam']
         k_abs = opac_dict['k_abs']
         k_sca = opac_dict['k_sca']
         g = opac_dict['g']
 
-        f = interp1d(np.log10(opac_dict['a']), np.array([np.log10(k_abs), np.log10(k_sca), g]), axis=1)
+        f = interp1d(np.log10(opac_dict['a']), np.array(
+            [np.log10(k_abs), np.log10(k_sca), g]), axis=1)
 
         lk_abs, lk_sca, g = f(np.log10(a_grain))
         k_abs = 10.**lk_abs
         k_sca = 10.**lk_sca
 
     write_radmc3d_dustkappa_from_array(name, lam, k_abs, k_sca, g, path=path)
 
@@ -2302,19 +2364,24 @@
 
     """
     filename = os.path.join(path, 'dustkapscatmat_{}.inp'.format(name))
 
     with open(filename, 'w') as f:
         f.write('# Opacity and scattering matrix file for ' + name + '\n')
         f.write('# Please do not forget to cite in your publications theo riginal paper of these optical constant measurements\n')
-        f.write('# Made with the DSHARP_OPAC package by Cornelis Dullemond & Til Birnstiel\n')
-        f.write('# using either the bhmie.py Mie code of Bohren and Huffman (python version by Cornelis Dullemond,\n')
-        f.write('# or a F90 version by Til Birnstiel, both after the original bhmie.f code by Bruce Draine)\n')
-        f.write('# Grain size = {0:13.6e} cm\n'.format(opacity_dict["a"][index]))
-        f.write('# Material density = {0:6.3f} g/cm^3\n'.format(opacity_dict["rho_s"]))
+        f.write(
+            '# Made with the DSHARP_OPAC package by Cornelis Dullemond & Til Birnstiel\n')
+        f.write(
+            '# using either the bhmie.py Mie code of Bohren and Huffman (python version by Cornelis Dullemond,\n')
+        f.write(
+            '# or a F90 version by Til Birnstiel, both after the original bhmie.f code by Bruce Draine)\n')
+        f.write('# Grain size = {0:13.6e} cm\n'.format(
+            opacity_dict["a"][index]))
+        f.write(
+            '# Material density = {0:6.3f} g/cm^3\n'.format(opacity_dict["rho_s"]))
         f.write('1\n')  # Format number
         f.write('{0:d}\n'.format(opacity_dict["lam"].size))
         f.write('{0:d}\n'.format(opacity_dict["theta"].size))
         f.write('\n')
         for i in range(opacity_dict['lam'].size):
             f.write('%13.6e %13.6e %13.6e %13.6e\n' % (opacity_dict['lam'][i] * 1e4,
                                                        opacity_dict['k_abs'][index, i],
@@ -2324,15 +2391,16 @@
         for j in range(opacity_dict['theta'].size):
             f.write('%13.6e\n' % (opacity_dict['theta'][j]))
         f.write('\n')
         for ilam in range(opacity_dict['lam'].size):
             for itheta in range(opacity_dict['theta'].size):
                 f.write('%13.6e %13.6e %13.6e %13.6e %13.6e %13.6e\n' %
                         (opacity_dict['zscat'][index, ilam, itheta, 0], opacity_dict['zscat'][index, ilam, itheta, 1],
-                         opacity_dict['zscat'][index, ilam, itheta, 2], opacity_dict['zscat'][index, ilam, itheta, 3],
+                         opacity_dict['zscat'][index, ilam, itheta,
+                                               2], opacity_dict['zscat'][index, ilam, itheta, 3],
                          opacity_dict['zscat'][index, ilam, itheta, 4], opacity_dict['zscat'][index, ilam, itheta, 5]))
             f.write('\n')
 
 
 def interpolate_radmc3d_scatmat_file(a, opacity_dict, name, path='.'):
     """
     The RADMC-3D radiative transfer package[1] can perform dust continuum
@@ -2391,27 +2459,33 @@
     zscat = opacity_dict['zscat']
 
     filename = os.path.join(path, 'dustkapscatmat_{}.inp'.format(name))
 
     with open(filename, 'w') as f:
         f.write('# Opacity and scattering matrix file for ' + name + '\n')
         f.write('# Please do not forget to cite in your publications theo riginal paper of these optical constant measurements\n')
-        f.write('# Made with the DSHARP_OPAC package by Cornelis Dullemond & Til Birnstiel\n')
-        f.write('# using either the bhmie.py Mie code of Bohren and Huffman (python version by Cornelis Dullemond,\n')
-        f.write('# or a F90 version by Til Birnstiel, both after the original bhmie.f code by Bruce Draine)\n')
+        f.write(
+            '# Made with the DSHARP_OPAC package by Cornelis Dullemond & Til Birnstiel\n')
+        f.write(
+            '# using either the bhmie.py Mie code of Bohren and Huffman (python version by Cornelis Dullemond,\n')
+        f.write(
+            '# or a F90 version by Til Birnstiel, both after the original bhmie.f code by Bruce Draine)\n')
         f.write('# Grain size = {0:13.6e} cm\n'.format(a))
-        f.write('# Material density = {0:6.3f} g/cm^3\n'.format(opacity_dict["rho_s"]))
+        f.write(
+            '# Material density = {0:6.3f} g/cm^3\n'.format(opacity_dict["rho_s"]))
         f.write('1\n')  # Format number
         f.write('{0:d}\n'.format(opacity_dict["lam"].size))
         f.write('{0:d}\n'.format(opacity_dict["theta"].size))
         f.write('\n')
         for i in range(opacity_dict['lam'].size):
             f.write('%13.6e %13.6e %13.6e %13.6e\n' % (opacity_dict['lam'][i] * 1e4,
-                                                       np.interp(a, a_grid, opacity_dict['k_abs'][:, i]),
-                                                       np.interp(a, a_grid, opacity_dict['k_sca'][:, i]),
+                                                       np.interp(
+                                                           a, a_grid, opacity_dict['k_abs'][:, i]),
+                                                       np.interp(
+                                                           a, a_grid, opacity_dict['k_sca'][:, i]),
                                                        np.interp(a, a_grid, opacity_dict['g'][:, i])))
         f.write('\n')
         for j in range(opacity_dict['theta'].size):
             f.write('%13.6e\n' % (opacity_dict['theta'][j]))
         f.write('\n')
         for ilam in range(opacity_dict['lam'].size):
             for itheta in range(opacity_dict['theta'].size):
@@ -2463,15 +2537,16 @@
 
         theta = np.fromfile(f, dtype=float, count=n_theta, sep=' ')
 
         zscat = np.zeros([n_lam, n_theta, 6])
 
         for ilam in range(n_lam):
             for itheta in range(n_theta):
-                zscat[ilam, itheta, :] = np.fromfile(f, dtype=float, count=6, sep=' ')
+                zscat[ilam, itheta, :] = np.fromfile(
+                    f, dtype=float, count=6, sep=' ')
 
         while True:
             line = f.readline()
             if not line:
                 break
             elif line.strip() != '':
                 raise ValueError('there remain lines in the scatmat file!')
@@ -2552,27 +2627,30 @@
             for i in np.arange(nlam):
                 try:
                     nk[i] = c.nk(lam[i])
                 except BaseException:
                     nk[i] = np.nan
 
         mask = np.invert(np.isnan(nk[:, 0]))
-        lines += ax1.loglog(lam[mask], nk[:, 0][mask], label='$n_1$ - {}'.format(c.material_str), alpha=0.7, ls='-')
+        lines += ax1.loglog(lam[mask], nk[:, 0][mask],
+                            label='$n_1$ - {}'.format(c.material_str), alpha=0.7, ls='-')
         mask = np.invert(np.isnan(nk[:, 1]))
-        lines += ax2.loglog(lam[mask], nk[:, 1][mask], label='$k_1$ - {}'.format(c.material_str), c=lines[-1].get_color(), alpha=0.7, ls='--')
+        lines += ax2.loglog(lam[mask], nk[:, 1][mask], label='$k_1$ - {}'.format(
+            c.material_str), c=lines[-1].get_color(), alpha=0.7, ls='--')
 
     ax1.set_xlabel('wavelength [cm]')
     if twoaxes:
         ax1.set_ylabel('$n$')
         ax2.set_ylabel('$k$')
         ax1.set_yscale('linear')
     else:
         ax1.set_ylabel('$n, k$')
 
-    ax1.legend(lines, [li.get_label() for li in lines], loc='best', fontsize='xx-small')
+    ax1.legend(lines, [li.get_label()
+               for li in lines], loc='best', fontsize='xx-small')
 
     if twoaxes:
         return ax1, ax2
     else:
         return ax1
 
 
@@ -2641,25 +2719,28 @@
 
     f_vol = rho_s / densities * f_mass
     f_vol = f_vol / f_vol.sum()
 
     length = max([len(c.material_str) for c in constants])
     length = max([length, 16])
 
-    print('| material'.ljust(length + 2) + '| volume fractions | mass fractions |')
+    print('| material'.ljust(length + 2) +
+          '| volume fractions | mass fractions |')
     print('|' + (length + 1) * '-' + '|' + 18 * '-' + '|' + 16 * '-' + '|')
     for c, fv, fm in zip(constants, f_vol, f_mass):
-        print('| ' + c.material_str.ljust(length) + '| {:.4}'.format(fv).ljust(19) + '| {:.4}'.format(fm).ljust(17) + '|')
+        print('| ' + c.material_str.ljust(length) +
+              '| {:.4}'.format(fv).ljust(19) + '| {:.4}'.format(fm).ljust(17) + '|')
 
     # mix the optical constants using the Bruggeman rule
 
     diel_const = diel_mixed(constants, f_vol, rule=rule)
 
     if porosity > 0:
-        diel_const = diel_mixed([diel_vacuum(), diel_const], [porosity, (1 - porosity)], rule='Maxwell-Garnett')
+        diel_const = diel_mixed([diel_vacuum(), diel_const], [
+                                porosity, (1 - porosity)], rule='Maxwell-Garnett')
         rho_s *= 1 - porosity
 
     return diel_const, rho_s
 
 
 def get_ricci_mix(extrapol=False, lmax=None, rule='Bruggeman'):
     """
@@ -2770,16 +2851,19 @@
                 # k_sca[grain, i] = integral
 
                 # g = <mu> = 2 pi / kappa * int(Z11(mu) mu dmu)
                 # mu_av = 0.5 * (mu[1:] + mu[:-1])
                 # P_mu = 2 * np.pi / k_sca[grain, i] * 0.5 * (zscat[grain, i, 1:, 0] + zscat[grain, i, :-1, 0])
                 # g[grain, i] = np.sum(P_mu * mu_av * dmu)
 
-                k_sca[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0], x=mu)
-                g[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0] * mu, x=mu) / k_sca[grain, i]
+                k_sca[grain, i] = -2 * np.pi * \
+                    np.trapz(zscat[grain, i, :, 0], x=mu)
+                g[grain, i] = -2 * np.pi * \
+                    np.trapz(zscat[grain, i, :, 0] *
+                             mu, x=mu) / k_sca[grain, i]
 
     return zscat, zscat_nochop, k_sca, g
 
 
 def get_opacities(a, lam, rho_s, diel_const, bhmie_function=bhmie_function,
                   extrapol=False, n_angle=3,
                   extrapolate_large_grains=False):
@@ -2936,15 +3020,16 @@
         g_i = f_g(lam_avg, a).T
 
     # - scattering amplitudes
 
     if S1 is not None:
         n_th = S1.shape[-1]
         th = np.arange(n_th, dtype=float)
-        new_points = np.reshape(np.meshgrid(a, lam_avg, th, indexing='ij'), (3, -1), order='C').T
+        new_points = np.reshape(np.meshgrid(
+            a, lam_avg, th, indexing='ij'), (3, -1), order='C').T
 
         f_S1 = RegularGridInterpolator((a, lam, th), S1)
         S1_i = f_S1(new_points).reshape([len(a), len(lam_avg), len(th)])
 
         f_S2 = RegularGridInterpolator((a, lam, th), S2)
         S2_i = f_S2(new_points).reshape([len(a), len(lam_avg), len(th)])
 
@@ -2984,24 +3069,27 @@
     if S1 is not None:
         ret['S1'] = S1_m
         ret['S2'] = S2_m
 
     # calculate beta
 
     if calc_beta:
-        beta = -np.log10(ka[-1, :] / ka[0, :]) / np.log10(lam_avg[-1] / lam_avg[0])
+        beta = -np.log10(ka[-1, :] / ka[0, :]) / \
+            np.log10(lam_avg[-1] / lam_avg[0])
         ret['beta'] = beta
 
     if plot:
         if ax is None:
             _, ax = plt.subplots()
         ax = np.array(ax, ndmin=1)
         lines = []
-        lines += ax[0].loglog(a, ka[0, :], '-', label=r'absorption, $\lambda = {:2.2g}$ mm'.format(lam_avg[0] * 10))
-        lines += ax[0].loglog(a, ks[0, :], '--', label=r'scattering, $\lambda = {:2.2g}$ mm'.format(lam_avg[0] * 10))
+        lines += ax[0].loglog(a, ka[0, :], '-',
+                              label=r'absorption, $\lambda = {:2.2g}$ mm'.format(lam_avg[0] * 10))
+        lines += ax[0].loglog(a, ks[0, :], '--',
+                              label=r'scattering, $\lambda = {:2.2g}$ mm'.format(lam_avg[0] * 10))
         ax[0].set_xlabel(r'$a_\mathrm{max}$ [cm]')
         ax[0].set_ylabel(r'$\kappa$ [cm$^2$/g]')
         ax[0].set_xlim(1e-4, 1e2)
         ax[0].set_ylim(0.01, 50)
 
         one_leg = True
         lines2 = []
@@ -3065,15 +3153,16 @@
 
     # number of finer grid points around each grid.
 
     n_inter = 40
 
     # for gaussian smoothing:
     eps = 0.1   # how far around each grid point the averaging-grid extends
-    sigma = 0.05  # the width of the gaussian weights around a[i] (in terms of a[i])
+    # the width of the gaussian weights around a[i] (in terms of a[i])
+    sigma = 0.05
 
     if smoothing == 'linear':
 
         # define a delta-a which tells us how much down and up we go around each grid point.
         # the factor (n_inter - 1) / n_inter is to avoid overlapping intervals
 
         da = np.diff(a) / 2. * (n_inter - 1) / n_inter
@@ -3091,18 +3180,20 @@
         raise ValueError('smoothing must be \'gaussian\' or \'linear\'')
 
     # make the fine linear particle size grid. All these *fine linear*
     # calculations have the suffix `_h`.
 
     a_h = np.array([])
     for i in range(len(a)):
-        a_h = np.hstack((a_h, np.linspace(a[i] - da[i], a[i] + da[i], n_inter)))
+        a_h = np.hstack(
+            (a_h, np.linspace(a[i] - da[i], a[i] + da[i], n_inter)))
 
     if np.any(a_h < 0):
-        raise ValueError('particle size smaller 0, please increase particle size grid resolution')
+        raise ValueError(
+            'particle size smaller 0, please increase particle size grid resolution')
 
     # calculate the high res opacities
 
     res_h = get_opacities(a_h, lam, rho_s, diel_const, **kwargs)
 
     k_abs_h = res_h['k_abs']
     k_sca_h = res_h['k_sca']
```

### Comparing `dsharp_opac-1.1.7/dsharp_opac/fit_module.f90` & `dsharp_opac-1.1.8rc0/dsharp_opac/fit_module.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/links.json` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/draine/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/links.json` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/new/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/links.json` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/henning/old/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/silicate.dat` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/luca/silicate.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/make_lnk.py` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/pollack1994/make_lnk.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/beta.dat` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/beta.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/warren_1984.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf` & `dsharp_opac-1.1.8rc0/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/AppendixB.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/AppendixB.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure1.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure1.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure2.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure2.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure3.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure3.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure4.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure4.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure56.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure56.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure7.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure7.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/Figure8.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure8.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.866170634920635%*

 * *Differences: {"'cells'": "{5: {'metadata': {replace: OrderedDict()}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3'}, 'language_info': {'version': "*

 * *               "'3.6.6'}}",*

 * * "'nbformat_minor'": '2'}*

```diff
@@ -67,17 +67,15 @@
                 "\n",
                 "Bnu    = np.array([aux.planck_B_nu(nu, T) for T in T_array])\n",
                 "dBnudT = np.array([aux.planck_dBnu_dT(nu, T) for T in T_array])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "source": [
                 "## Calculate mean opacities for all temperatures\n",
                 "\n",
                 "For the Rosseland Mean, we need the *extinction opacity*\n",
                 "\n",
                 "$$\n",
                 "\\kappa_\\nu^\\mathrm{ext}(a) = \\kappa_\\nu^{abs}(a) + (1-g)\\,\\kappa_\\nu^{sca}(a)\n",
@@ -337,27 +335,27 @@
                 "    )\n",
                 "f.savefig('figures/fig8_mean_opacities.pdf')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.6.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `dsharp_opac-1.1.7/notebooks/Figure9.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/Figure9.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/aux_functions.py` & `dsharp_opac-1.1.8rc0/notebooks/aux_functions.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/dsharp_porosity.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/dsharp_porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/index.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/opac_widget.py` & `dsharp_opac-1.1.8rc0/notebooks/opac_widget.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/opacity_examples.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/opacity_examples.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/opacity_package_tests.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/opacity_package_tests.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/polarization_fraction.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/polarization_fraction.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/porosity.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.7/notebooks/rosseland_mean_opacities.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/scattering_phase_functions.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7949423363095238%*

 * *Differences: {"'cells'": "{2: {'source': ['Define a plotting helper function'], delete: ['id']}, 5: {'source': "*

 * *            "['def hg(mu, g):\\n', '    return (1 - g**2) / (1 + g**2 - 2 * g * mu)**1.5'], "*

 * *            "delete: ['id']}, 7: {'metadata': {replace: OrderedDict()}, 'source': ['Set wavelength "*

 * *            "and sizes'], delete: ['id']}, 8: {'source': ['lam = np.array([0.55e-4])      # "*

 * *            "wavelength\\n', 'a   = np.array([1e-4, 10e-4])  # particle radius'], delete: ['id']}, "*

 * *            "10: {'sou […]*

```diff
@@ -1,250 +1,275 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "614a2e59-a741-4394-a90a-2d9093b6e8e8",
             "metadata": {},
             "source": [
-                "# Compute Rosseland Mean Opacity with `dsharp_opac`"
+                "# Scattering Phase Functions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9b60c0ac-e532-4258-bb79-4ee71130faf0",
-            "metadata": {},
+            "metadata": {
+                "slideshow": {
+                    "slide_type": "subslide"
+                }
+            },
             "outputs": [],
             "source": [
-                "import dsharp_opac as opacity\n",
+                "%matplotlib inline\n",
                 "import numpy as np\n",
-                "import matplotlib.pyplot as plt"
+                "import matplotlib.pyplot as plt\n",
+                "import seaborn as sns\n",
+                "\n",
+                "import pymiecoated\n",
+                "import dsharp_opac as opacity\n",
+                "\n",
+                "sns.set({'figure.dpi':200})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Define a plotting helper function"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def plot_logpolar(ax, theta, r_, bullseye=None, **kwargs):\n",
+                "    min10 = np.log10(np.min(r_))\n",
+                "    max10 = np.log10(np.max(r_))\n",
+                "    if bullseye is None:\n",
+                "        bullseye = min10 - np.log10(0.5 * np.min(r_))\n",
+                "    r = np.log10(r_) - min10 + bullseye\n",
+                "    ax.plot(theta, r, **kwargs)\n",
+                "    l = np.arange(np.floor(min10), max10)\n",
+                "    ax.set_rticks(l - min10 + bullseye) \n",
+                "    ax.set_yticklabels([\"$10^{{{:.0f}}}$\".format(x) for x in l],fontdict={'fontsize':'xx-small'})\n",
+                "    ax.set_rlim(0, max10 - min10 + bullseye)\n",
+                "    return ax"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "22a75cf8-7b53-4a0c-8153-a03b098d74f2",
             "metadata": {
-                "tags": []
+                "slideshow": {
+                    "slide_type": "-"
+                }
             },
             "source": [
-                "## Calculate mean opacities for all temperatures\n",
-                "\n",
-                "For the Rosseland Mean, we need the *extinction opacity*\n",
-                "\n",
-                "$$\n",
-                "\\kappa_\\nu^\\mathrm{ext}(a) = \\kappa_\\nu^{abs}(a) + (1-g)\\,\\kappa_\\nu^{sca}(a)\n",
-                "$$\n",
-                "\n",
-                "then the total opacity of the size distribution is given by\n",
-                "\n",
-                "$$\n",
-                "\\kappa_\\nu^\\mathrm{abs,tot} = \\frac{\\int_0^{a_\\mathrm{max}} n(a)\\,m\\,\\kappa_\\nu^\\mathrm{abs}(a) \\,\\mathrm{d}a}{\\int_0^{a_\\mathrm{max}} n(a)\\,m \\,\\mathrm{d}a}\n",
-                "$$\n",
-                "\n",
-                "The Planck mean opacity is \n",
-                "\n",
-                "$$\n",
-                "\\bar \\kappa_\\mathrm{P}(T) = \\frac{\\int_0^\\infty \\kappa_\\nu^\\mathrm{abs,tot}\\, B_\\nu(T)\\,\\mathrm{d}\\nu}{\\int_0^\\infty  B_\\nu(T)\\,\\mathrm{d}\\nu}\n",
-                "$$\n",
-                "\n",
-                "and the Rosseland mean opacity is\n",
-                "\n",
-                "$$\n",
-                "\\bar \\kappa_\\mathrm{R}(T) = \\left( \\frac{\\int_0^\\infty \\frac{1}{\\kappa_\\nu^\\mathrm{ext,tot}} \\, \\frac{\\mathrm{d}B_\\nu(T)}{\\mathrm{d}T}\\,\\mathrm{d}\\nu}{\\int_0^\\infty  \\frac{\\mathrm{d}B_\\nu(T)}{\\mathrm{d}T}\\,\\mathrm{d}\\nu}\\right)^{-1}\n",
-                "$$"
+                "Define the Henyey-Greenstein phase function"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "415862ae-1366-4209-b7b2-960890dd020e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with np.load(opacity.get_datafile('default_opacities_smooth.npz')) as d:\n",
-                "    a      = d['a']\n",
-                "    g      = d['g']\n",
-                "    lam    = d['lam']\n",
-                "    k_abs  = d['k_abs']\n",
-                "    k_sca  = d['k_sca']"
+                "def hg(mu, g):\n",
+                "    return (1 - g**2) / (1 + g**2 - 2 * g * mu)**1.5"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "slideshow": {
+                    "slide_type": "slide"
+                }
+            },
+            "source": [
+                "## Calculate liquid water phase function"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Set wavelength and sizes"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a2fa1186-3fb5-472d-9640-8dcfde87b484",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def planck_dBnu_dT(freq, T):\n",
-                "    \"\"\"This function computes the temperature derivative of the blackbody function\n",
-                "\n",
-                "            dB_nu(T)        2 h^2 nu^4      exp(h nu / kT)        1\n",
-                "            --------   =    ---------- ------------------------  ---\n",
-                "               dT            k c^2    [ exp(h nu / kT) - 1 ]^2  T^2\n",
-                "\n",
-                "    Arguments\n",
-                "    ---------\n",
-                "\n",
-                "    freq : float or array\n",
-                "        frequency [in Hz or with astropy.units]\n",
-                "\n",
-                "    temp : float or array\n",
-                "        temperature [in K or with astropy.units]\n",
-                "\n",
-                "    Returns:\n",
-                "    --------\n",
-                "    dBdT: the temperature derivative of the planck spectrum\n",
-                "        units are using astropy.units if the input values use those, otherwise\n",
-                "        cgs units: erg/(K*s*sr*cm**2*Hz)\n",
-                "\n",
-                "    \"\"\"\n",
-                "    if isinstance(T, u.quantity.Quantity):\n",
-                "        use_units = True\n",
-                "    else:\n",
-                "        T = T * u.K\n",
-                "        use_units = False\n",
-                "\n",
-                "    if not isinstance(freq, u.quantity.Quantity):\n",
-                "        freq = freq * u.Hz\n",
-                "\n",
-                "    T = np.array(T.value, ndmin=1) * T.unit\n",
-                "    freq = np.array(freq.value, ndmin=1) * freq.unit\n",
-                "\n",
-                "    f_ov_T = freq[np.newaxis, :] / T[:, np.newaxis]\n",
-                "    mx = np.floor(np.log(np.finfo(f_ov_T.ravel()[0].value).max))\n",
-                "    exp = np.minimum(f_ov_T * c.h / c.k_B, mx)\n",
-                "    exp = np.maximum(exp, -mx)\n",
-                "    exp = np.exp(exp)\n",
-                "\n",
-                "    dBdT = 2 * c.h**2 * freq[np.newaxis, :]**4 / (c.k_B * c.c**2 * T[:, np.newaxis]**2) * \\\n",
-                "        1. / (exp * (1. - 1. / exp)**2) / u.sr\n",
-                "\n",
-                "    cgsunit = 'erg/(s*Hz*sr*cm**2*K)'\n",
-                "    if use_units:\n",
-                "        return dBdT.to(cgsunit).squeeze()\n",
-                "    else:\n",
-                "        return dBdT.to(cgsunit).value.squeeze()"
+                "lam = np.array([0.55e-4])      # wavelength\n",
+                "a   = np.array([1e-4, 10e-4])  # particle radius"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a7774020-f790-4655-8c14-5612783fefb9",
             "metadata": {},
             "source": [
-                "**here you should interpolate onto your dustpy size grid**"
+                "Calculate Mie opacities"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "da66ed97-de91-4f4e-8855-513959414cba",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# define temperature and wavelength arrays\n",
+                "dc = opacity.diel_segelstein_water()\n",
+                "rho_s = dc.rho\n",
+                "result = opacity.get_opacities(a, lam, rho_s=rho_s, diel_const=dc, n_angle=500)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Make polar and regular plots of the phase function and overplot the HG phase function"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "f1,ax1 = plt.subplots(1, 2, figsize=(12, 5), subplot_kw=dict(projection='polar'))\n",
+                "f2,ax2 = plt.subplots(1, 2, figsize=(12, 3))\n",
+                "\n",
+                "for ia in range(len(a)):\n",
+                "    g     = result['g'][ia, 0]\n",
+                "    S1    = result['S1'][ia, 0, :]\n",
+                "    S2    = result['S2'][ia, 0, :]\n",
+                "    theta = result['theta']\n",
+                "    angle = theta * np.pi / 180.\n",
+                "    mu    = np.cos(angle)\n",
+                "    m     = 4 * np.pi / 3 * rho_s * a[ia]**3\n",
                 "\n",
-                "T_array = np.logspace(0, np.log10(1500), 250)\n",
-                "nu = c.c.cgs.value / lam\n",
+                "    sig_s = result['q_sca'][ia, 0] * np.pi * a[ia]**2\n",
+                "    sig_a = result['q_abs'][ia, 0] * np.pi * a[ia]**2\n",
                 "\n",
-                "# calculate the planck function and their derivatives for all those temperatures and wavelength\n",
+                "    S11   = 0.5 * (S1 * S1.conjugate() + S2 * S2.conjugate()).real\n",
+                "    P11   = lam**2 / (np.pi * sig_s) * S11\n",
                 "\n",
-                "dBnudT = np.array([planck_dBnu_dT(nu, T) for T in T_array])"
+                "\n",
+                "    plot_logpolar(ax1[ia], angle, hg(mu,g), label='Henyey-Greenstein')\n",
+                "    plot_logpolar(ax1[ia], angle, P11, label='Mie calculation',lw=1)\n",
+                "\n",
+                "\n",
+                "    ax2[ia].semilogy(theta, hg(mu,g), label='Henyey-Greenstein')\n",
+                "    ax2[ia].semilogy(theta, P11, label='Mie calculation',lw=1)\n",
+                "\n",
+                "\n",
+                "for _ax in ax1:\n",
+                "    _ax.set_thetamax(180)\n",
+                "    _ax.set_xticks(np.linspace(0,np.pi,5))\n",
+                "    _ax.legend();\n",
+                "    \n",
+                "for _ax in ax2:\n",
+                "    _ax.set_xticks([0, 50, 100, 150])\n",
+                "    _ax.legend();"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "slideshow": {
+                    "slide_type": "slide"
+                }
+            },
+            "source": [
+                "## Calculate M\u00fcller Matrix"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a1165078-389f-4e7d-a7de-cd2dbb997a63",
             "metadata": {},
             "outputs": [],
             "source": [
-                "k_ext = k_abs + (1 - g) * k_sca"
+                "theta = result['theta']\n",
+                "k_sca = result['k_sca']\n",
+                "S1    = result['S1']\n",
+                "S2    = result['S2']\n",
+                "lam   = result['lam']\n",
+                "g     = result['g']"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9c2a7dea-c44f-484a-8a24-7658212f8c9b",
             "metadata": {},
             "source": [
-                "**here we use a power-law, replace it with dustpy size distribution**\n",
-                "make sure to normalize it"
+                "Calculate the masses and the M\u00fcller matrix"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dcca5607-b808-4d83-aa82-680546755aeb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "q = 3.5\n",
-                "amax = 0.1\n",
-                "power_law = a**(4 - q)\n",
-                "power_law[a > amax] = 0\n",
-                "power_law = power_law / power_law.sum()"
+                "m  = 4 * np.pi / 3 * rho_s * a**3\n",
+                "MM = opacity.calculate_mueller_matrix(lam, m, S1, S2, theta=theta, k_sca=k_sca)\n",
+                "zscat = MM['zscat']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6ccaf2e7-37b6-4a95-8a5b-b8428277b2c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "k_R_p  = np.zeros_like(T_array)\n",
-                "\n",
-                "# for each temperature ...\n",
-                "\n",
-                "for it, T in enumerate(T_array):\n",
-                "    \n",
-                "    # sum the absorption opacity\n",
-                "\n",
-                "    k_abs_p = (k_abs * power_law[:, None]).sum(0)\n",
-                "\n",
-                "    # sum the EXTINCTION opacity\n",
-                "\n",
-                "    k_ext_p = (k_ext * power_law[:, None]).sum(0)\n",
-                "    \n",
-                "    # calculate Rosseland opacity for the fit and the power-law\n",
-                "    \n",
-                "    B   = np.trapz(dBnudT[it, :], x=nu)\n",
-                "    k_R_p[it]  = B / np.trapz(dBnudT[it, :].T / k_ext_p, x=nu)"
+                "mu = np.cos(np.pi * theta / 180)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "For some selected sizes and wavelengths: check conventions of $Z_{11}$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eedf0f15-2830-45c4-a556-726e7468ca89",
             "metadata": {},
             "outputs": [],
             "source": [
-                "f, ax = plt.subplots()\n",
-                "ax.loglog(T_array, k_R_p)\n",
-                "ax.set_xlabel('T [K]')\n",
-                "ax.set_xlabel('$\\kappa_R$ [cm$^2$/g]');"
+                "ia = 1\n",
+                "ilam = 0\n",
+                "\n",
+                "kk = 2 * np.pi * np.trapz(zscat[ia, ilam, ::-1, 0], x=mu[::-1])\n",
+                "gg = 2 * np.pi / kk * np.trapz(mu[::-1] * zscat[ia, ilam, ::-1, 0], x=mu[::-1])\n",
+                "\n",
+                "\n",
+                "print('k_sca[Z11] = {:.6g}'.format(ks))\n",
+                "print('k_sca[Mie] = {:.6g}'.format(k_sca[ia, ilam]))\n",
+                "print('g[Z11]     = {:.6g}'.format(gg))\n",
+                "print('g[Mie]     = {:.6g}'.format(g[ia, ilam]))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.6.8"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `dsharp_opac-1.1.7/notebooks/smoothed_opacities.ipynb` & `dsharp_opac-1.1.8rc0/notebooks/smoothed_opacities.ipynb`

 * *Files identical despite different names*

