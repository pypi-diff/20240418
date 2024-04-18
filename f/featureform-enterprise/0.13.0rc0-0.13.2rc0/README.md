# Comparing `tmp/featureform_enterprise-0.13rc0.tar.gz` & `tmp/featureform_enterprise-0.13.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform_enterprise-0.13rc0.tar", last modified: Fri Apr 12 17:57:42 2024, max compression
+gzip compressed data, was "featureform_enterprise-0.13.2rc0.tar", last modified: Thu Apr 18 17:40:11 2024, max compression
```

## Comparing `featureform_enterprise-0.13rc0.tar` & `featureform_enterprise-0.13.2rc0.tar`

### file list

```diff
@@ -1,400 +1,401 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.609729 featureform_enterprise-0.13rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-12 17:57:42.609729 featureform_enterprise-0.13rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 17:57:42.609729 featureform_enterprise-0.13rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.529729 featureform_enterprise-0.13rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.537729 featureform_enterprise-0.13rc0/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    40294 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.525729 featureform_enterprise-0.13rc0/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.537729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.537729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.525729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.529729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.537729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.537729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.581729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
--rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
--rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
--rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.589729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
--rw-r--r--   0 runner    (1001) docker     (127)  4221291 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-ff28ddf757476fd7.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/query-f3c47b8d51f1458e.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/search-e03b34f74065bab5.js
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-31dc8fc1d5040dae.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/group/[groupName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/groups.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/role/[roleName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.593729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/user/[userName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/users.html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/query.html
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.601729 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    61862 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/base_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/clearIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/creature.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/localmode.png
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/welcomebackground.png
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-12 17:57:38.000000 featureform_enterprise-0.13rc0/src/featureform/dashboard/out/tasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.601729 featureform_enterprise-0.13rc0/src/featureform/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.601729 featureform_enterprise-0.13rc0/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-12 17:56:01.000000 featureform_enterprise-0.13rc0/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-12 17:56:01.000000 featureform_enterprise-0.13rc0/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (127)   198068 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    83137 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    36948 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/status_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/variant_names_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.609729 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34473 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 17:57:42.000000 featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:57:42.609729 featureform_enterprise-0.13rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_autogenerated_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    44163 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_multi_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_source_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_training_set_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-12 17:55:18.000000 featureform_enterprise-0.13rc0/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.219948 featureform_enterprise-0.13.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-18 17:40:11.219948 featureform_enterprise-0.13.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-18 17:40:11.219948 featureform_enterprise-0.13.2rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.139949 featureform_enterprise-0.13.2rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.147949 featureform_enterprise-0.13.2rc0/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40264 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.139949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.147949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.147949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.139949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.139949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.147949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.151949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.195948 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4221319 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-d61fafb974c05741.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/query-f3c47b8d51f1458e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/search-e03b34f74065bab5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.203949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.207949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.207949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/group/[groupName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/groups.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.207949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/role/[roleName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.207949 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/user/[userName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.211948 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    61862 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/base_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/clearIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/creature.png
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/localmode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/welcomebackground.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-18 17:40:06.000000 featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.211948 featureform_enterprise-0.13.2rc0/src/featureform/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.215948 featureform_enterprise-0.13.2rc0/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-18 17:38:38.000000 featureform_enterprise-0.13.2rc0/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-18 17:38:38.000000 featureform_enterprise-0.13.2rc0/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (127)   200019 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84058 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/variant_names_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.219948 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 17:40:11.000000 featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:11.219948 featureform_enterprise-0.13.2rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_autogenerated_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_multi_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_source_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_training_set_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-18 17:37:55.000000 featureform_enterprise-0.13.2rc0/tests/test_updating_provider.py
```

### Comparing `featureform_enterprise-0.13rc0/LICENSE` & `featureform_enterprise-0.13.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/PKG-INFO` & `featureform_enterprise-0.13.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.0rc0
+Version: 0.13.2rc0
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13rc0/README.md` & `featureform_enterprise-0.13.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/setup.cfg` & `featureform_enterprise-0.13.2rc0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform-enterprise
-version = 0.13.0-rc0
+version = 0.13.2-rc
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Enterprise Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls =
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/__init__.py` & `featureform_enterprise-0.13.2rc0/src/featureform/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,35 +20,36 @@
 from .serving import ServingClient
 from .resources import (
     DatabricksCredentials,
     EMRCredentials,
     AWSStaticCredentials,
     AWSAssumeRoleCredentials,
     GCPCredentials,
+    GlueCatalog,
     SparkCredentials,
     BasicCredentials,
     KerberosCredentials,
 )
 from .client import Client
 from .enums import ResourceType
 
 ServingClient = ServingClient
 ResourceClient = ResourceClient
 Client = Client
 
-
 # Executor Credentials
 DatabricksCredentials = DatabricksCredentials
 EMRCredentials = EMRCredentials
 SparkCredentials = SparkCredentials
 
 # Cloud Provider Credentials
 AWSStaticCredentials = AWSStaticCredentials
 AWSAssumeRoleCredentials = AWSAssumeRoleCredentials
 GCPCredentials = GCPCredentials
+GlueCatalog = GlueCatalog
 
 # HDFS Credentials
 BasicCredentials = BasicCredentials
 KerberosCredentials = KerberosCredentials
 
 # Class API
 Feature = FeatureColumnResource
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/cli.py` & `featureform_enterprise-0.13.2rc0/src/featureform/cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/client.py` & `featureform_enterprise-0.13.2rc0/src/featureform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             source (Union[SourceRegistrar, SubscriptableTransformation, str]): The source or transformation to compute the dataframe from
             variant (str): The source variant; can't be None if source is a string
             resource_type (ResourceType): The type of resource; can be one of ff.SOURCE, ff.FEATURE, ff.LABEL, or ff.TRAINING_SET
         """
         if isinstance(source, (SourceRegistrar, SubscriptableTransformation)):
             name, variant = source.name_variant()
             resource_type = ResourceType.SOURCE
-        elif isinstance(source, featureform.resources.TrainingSetVariant):
+        elif isinstance(source, TrainingSetVariant):
             name = source.name
             variant = source.variant
             resource_type = ResourceType.TRAINING_SET
         elif isinstance(source, str):
             name = source
             if variant is None:
                 raise ValueError("variant must be specified if source is a string")
@@ -283,15 +283,15 @@
 
         else:
             raise ValueError(
                 f"source must be of type SourceRegistrar, SubscriptableTransformation or str, not {type(resource)}\n"
                 "use client.dataframe(name, variant) or client.dataframe(source) or client.dataframe(transformation)"
             )
 
-        location = self.impl.location(name, variant, resource_type)
+        location = self.impl.path(name, variant, resource_type)
         return location
 
     def location(
         self,
         source: Union[SourceRegistrar, SubscriptableTransformation, str],
         variant: Optional[str] = None,
         resource_type: Optional[ResourceType] = None,
@@ -331,15 +331,15 @@
 
         else:
             raise ValueError(
                 f"source must be of type SourceRegistrar, SubscriptableTransformation or str, not {type(resource)}\n"
                 "use client.dataframe(name, variant) or client.dataframe(source) or client.dataframe(transformation)"
             )
 
-        location = self.impl.location(name, variant, resource_type)
+        location = self.impl.path(name, variant, resource_type)
         return location
 
     def close(self):
         """
         Closes the client, closes channel for hosted mode
         """
         self.impl.close()
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/404.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/group/[groupName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/[type]/[entity].html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-44302760e55a8032.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/search-e03b34f74065bab5.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/[type].html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/[type].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -12,12 +12,12 @@
     "/admin/role/[roleName]": ["static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js"],
     "/admin/roles": ["static/chunks/pages/admin/roles-a560426c6514c003.js"],
     "/admin/user/[userName]": ["static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js"],
     "/admin/users": ["static/chunks/pages/admin/users-313d4735cfc2c71a.js"],
     "/connections": ["static/chunks/pages/connections-f98076127418a04b.js"],
     "/query": ["static/chunks/pages/query-f3c47b8d51f1458e.js"],
     "/search": ["static/chunks/pages/search-e03b34f74065bab5.js"],
-    "/tasks": ["static/chunks/pages/tasks-31dc8fc1d5040dae.js"],
+    "/tasks": ["static/chunks/pages/tasks-cb5a5f315eeb0c01.js"],
     "/[type]": ["static/chunks/pages/[type]-7bfcb609b1affd61.js"],
     "/[type]/[entity]": ["static/chunks/pages/[type]/[entity]-44302760e55a8032.js"],
     sortedPages: ["/", "/404", "/_app", "/_error", "/admin/group/[groupName]", "/admin/groups", "/admin/role/[roleName]", "/admin/roles", "/admin/user/[userName]", "/admin/users", "/connections", "/query", "/search", "/tasks", "/[type]", "/[type]/[entity]"]
 }, self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-ff28ddf757476fd7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-d61fafb974c05741.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -98283,27 +98283,30 @@
                             title: "Groups",
                             urlPath: "/admin/groups",
                             icon: (0, l.jsx)(eC.Z, {})
                         }, ];
                     return (0, l.jsx)(l.Fragment, {
                         children: t.map(function(a, t) {
                             return (0, l.jsx)(eb.ZP, {
+                                sx: {
+                                    padding: "0 0 0 0"
+                                },
                                 children: (0, l.jsxs)(ek.Z, {
                                     onClick: function(t) {
                                         return e(t, a.urlPath)
                                     },
                                     children: [(0, l.jsx)(eS.Z, {
-                                        style: {
-                                            padding: "0 0 0 1.5em !important"
+                                        sx: {
+                                            minWidth: "40px"
                                         },
                                         children: a.icon
                                     }), (0, l.jsx)(ey.Z, {
                                         primary: a.title
                                     })]
-                                })
+                                }, t)
                             }, t)
                         })
                     })
                 },
                 eM = function(e) {
                     return {
                         sections: e.homePageSections
@@ -98376,34 +98379,37 @@
                                     },
                                     variant: "permanent",
                                     anchor: "left",
                                     children: [(0, l.jsxs)(ex.Z, {
                                         children: [null == a ? void 0 : a.features.map(function(e, a) {
                                             var t = eE.Z[e.type];
                                             return (0, l.jsx)(eb.ZP, {
+                                                sx: {
+                                                    padding: "0 0 0 0"
+                                                },
                                                 children: (0, l.jsxs)(ek.Z, {
                                                     onClick: function(e) {
                                                         return n(e, t.urlPath)
                                                     },
                                                     children: [(0, l.jsx)(eS.Z, {
-                                                        style: {
-                                                            padding: "0 0 0 1.5em !important"
+                                                        sx: {
+                                                            minWidth: "40px"
                                                         },
                                                         children: (0, l.jsx)(eh.Z, {
                                                             children: t.materialIcon
                                                         })
                                                     }), (0, l.jsx)(ey.Z, {
                                                         primary: t.typePlural
                                                     })]
                                                 })
                                             }, a)
                                         }), (0, l.jsxs)(ek.Z, {
                                             onClick: R,
                                             children: [(0, l.jsx)(eS.Z, {
-                                                style: {
+                                                sx: {
                                                     minWidth: "40px"
                                                 },
                                                 children: (0, l.jsx)(eh.Z, {
                                                     children: "all_inbox"
                                                 })
                                             }), (0, l.jsx)(ey.Z, {
                                                 primary: "Scheduling"
@@ -98417,32 +98423,35 @@
                                             component: "div",
                                             disablePadding: !0,
                                             children: (0, l.jsx)(ek.Z, {
                                                 onClick: function(e) {
                                                     return n(e, "/tasks")
                                                 },
                                                 sx: {
-                                                    padding: "0 0 0 4.5em"
+                                                    padding: "0 0 0.5em 4.5em"
                                                 },
                                                 children: (0, l.jsx)(ey.Z, {
                                                     primary: "Tasks"
                                                 })
                                             })
                                         })
                                     }), m && !1 !== i.rbacEnabled ? (0, l.jsxs)(l.Fragment, {
                                         children: [(0, l.jsx)(eg.Z, {}), (0, l.jsx)(eN, {})]
                                     }) : null, i.authEnabled && s ? (0, l.jsxs)(l.Fragment, {
                                         children: [(0, l.jsx)(eg.Z, {}), (0, l.jsx)(eb.ZP, {
+                                            sx: {
+                                                padding: "0 0 0 0"
+                                            },
                                             children: (0, l.jsxs)(ek.Z, {
                                                 onClick: function() {
                                                     return (0, p.signOut)()
                                                 },
                                                 children: [(0, l.jsx)(eS.Z, {
-                                                    style: {
-                                                        padding: "0 0 0 1.5em !important"
+                                                    sx: {
+                                                        minWidth: "40px"
                                                     },
                                                     children: (0, l.jsx)(ef.Z, {})
                                                 }), (0, l.jsx)(ey.Z, {
                                                     primary: "Sign Out"
                                                 })]
                                             })
                                         }, "signout")]
@@ -103855,15 +103864,14 @@
                         sx: {
                             paddingLeft: 0,
                             fontSize: 15
                         },
                         children: void 0 === n ? "" : n
                     }), (0, c.jsxs)(nz.Z, {
                         fullWidth: !0,
-                        maxWidth: "xl",
                         open: o,
                         onClose: x,
                         "aria-labelledby": "dialog-title",
                         "aria-describedby": "dialog-description",
                         children: [(0, c.jsxs)(nG.Z, {
                             id: "dialog-title",
                             "data-testid": "errorModalTitleId",
@@ -103885,14 +103893,17 @@
                                 onClick: x,
                                 children: (0, c.jsx)(nB.Z, {})
                             })]
                         }), (0, c.jsx)(nK.Z, {
                             children: (0, c.jsx)(L.Z, {
                                 variant: "body1",
                                 "data-testid": "fullTextContent",
+                                style: {
+                                    whiteSpace: "pre-line"
+                                },
                                 children: t
                             })
                         })]
                     })]
                 })
             }
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-31dc8fc1d5040dae.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -46,16 +46,16 @@
                 v = n(69397),
                 h = n(23972),
                 f = n(16003),
                 x = n(53640),
                 m = n(60076),
                 g = n(69587),
                 b = n(63931),
-                j = n(22715),
-                k = n(91057),
+                k = n(22715),
+                j = n(91057),
                 p = n(54799),
                 Z = n(21023),
                 R = n(66489),
                 w = n(310),
                 C = (0, n(45522).Z)(function() {
                     return {
                         inputRow: {
@@ -126,96 +126,98 @@
                     })[a]) && void 0 !== n ? n : "No Status"
                 })
             }
             var S = n(50594),
                 F = n(48263);
 
             function y(t) {
-                var e, n, r, o, d, v, f = t.handleClose,
-                    x = t.taskId,
-                    m = t.taskRunId,
-                    g = C(),
-                    b = (0, w.E)(),
-                    k = (0, a.useState)({}),
-                    I = k[0],
-                    y = k[1],
-                    E = (0, a.useState)(!0),
-                    A = E[0],
-                    L = E[1];
+                var e, n, r, o, d, v = t.handleClose,
+                    f = t.taskId,
+                    x = t.taskRunId,
+                    m = C(),
+                    g = (0, w.E)(),
+                    b = (0, a.useState)({}),
+                    j = b[0],
+                    I = b[1],
+                    y = (0, a.useState)(!0),
+                    E = y[0],
+                    A = y[1];
                 (0, a.useEffect)((0, l.Z)(function() {
                     var t, e, n;
                     return (0, s.__generator)(this, function(e) {
                         switch (e.label) {
                             case 0:
-                                if (t = null, !(x && m && A)) return [3, 2];
-                                return [4, b.getTaskRunDetails(x, m)];
+                                if (t = null, !(f && x && E)) return [3, 2];
+                                return [4, g.getTaskRunDetails(f, x)];
                             case 1:
-                                return y(e.sent()), n = setTimeout(function() {
-                                    L(!1)
+                                return I(e.sent()), n = setTimeout(function() {
+                                    A(!1)
                                 }, 750), [2, function() {
                                     n && clearTimeout(n)
                                 }];
                             case 2:
                                 return [2, function() {
                                     t && clearTimeout(t)
                                 }]
                         }
                     })
-                }), [x, m, A]);
-                var D = function() {
-                    A || L(!0)
+                }), [f, x, E]);
+                var L = function() {
+                    E || A(!0)
                 };
                 return (0, i.jsxs)(c.Z, {
-                    className: g.taskCardBox,
+                    className: m.taskCardBox,
                     children: [(0, i.jsxs)(c.Z, {
                         style: {
                             float: "right"
                         },
                         children: [(0, i.jsx)(Z.Z, {
                             title: "Refresh card",
                             placement: "bottom",
                             children: (0, i.jsx)(p.Z, {
                                 variant: "",
                                 size: "large",
-                                onClick: D,
-                                children: A ? (0, i.jsx)(R.Z, {
+                                onClick: L,
+                                children: E ? (0, i.jsx)(R.Z, {
                                     size: ".75em"
                                 }) : (0, i.jsx)(u.Z, {
                                     "data-testid": "taskRunRefreshIcon"
                                 })
                             })
                         }), (0, i.jsx)(p.Z, {
                             variant: "",
                             size: "large",
                             onClick: function() {
-                                return f()
+                                return v()
                             },
                             children: (0, i.jsx)(S.Z, {})
                         })]
                     }), (0, i.jsxs)(F.ZP, {
                         style: {
-                            padding: 12
+                            padding: 10
                         },
                         container: !0,
                         children: [(0, i.jsx)(F.ZP, {
                             item: !0,
-                            xs: 6,
+                            xs: 7,
                             justifyContent: "flex-start",
                             children: (0, i.jsx)(h.Z, {
                                 variant: "h5",
-                                children: null == I ? void 0 : null === (e = I.taskRun) || void 0 === e ? void 0 : e.name
+                                children: null !== (r = null == j ? void 0 : null === (e = j.taskRun) || void 0 === e ? void 0 : e.name) && void 0 !== r ? r : ""
                             })
                         }), (0, i.jsx)(F.ZP, {
                             item: !0,
-                            xs: 6,
+                            xs: 4,
                             justifyContent: "center",
                             children: (0, i.jsxs)(h.Z, {
                                 variant: "h6",
-                                children: ["Status: ", (0, i.jsx)(T, {
-                                    status: null == I ? void 0 : null === (n = I.taskRun) || void 0 === n ? void 0 : n.status
+                                children: [(0, i.jsx)("strong", {
+                                    children: "Status:"
+                                }), " ", (0, i.jsx)(T, {
+                                    status: null !== (o = null == j ? void 0 : null === (n = j.taskRun) || void 0 === n ? void 0 : n.status) && void 0 !== o ? o : ""
                                 })]
                             })
                         }), (0, i.jsx)(F.ZP, {
                             item: !0,
                             xs: 12,
                             justifyContent: "flex-start",
                             style: {
@@ -225,21 +227,25 @@
                                 variant: "h6",
                                 children: "Logs/Errors"
                             })
                         }), (0, i.jsx)(F.ZP, {
                             item: !0,
                             xs: 12,
                             justifyContent: "flex-start",
-                            children: (0, i.jsx)(j.Z, {
+                            children: (0, i.jsx)(k.Z, {
                                 style: {
                                     width: "100%"
                                 },
                                 variant: "filled",
                                 disabled: !0,
-                                value: (null == I ? void 0 : null === (r = I.taskRun) || void 0 === r ? void 0 : null === (o = r.logs) || void 0 === o ? void 0 : o.join("\n")) + "\n" + (null == I ? void 0 : null === (d = I.taskRun) || void 0 === d ? void 0 : d.error),
+                                value: function() {
+                                    var t, e, n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
+                                        i = "";
+                                    return (null == n ? void 0 : null === (t = n.taskRun) || void 0 === t ? void 0 : t.logs) && (i += n.taskRun.logs.join("\n")), (null == n ? void 0 : null === (e = n.taskRun) || void 0 === e ? void 0 : e.error) && (i += "\n" + n.taskRun.error), i
+                                }(j),
                                 multiline: !0,
                                 minRows: 3
                             })
                         }), (0, i.jsx)(F.ZP, {
                             item: !0,
                             xs: 12,
                             justifyContent: "flex-start",
@@ -266,15 +272,15 @@
                                     "& .MuiDataGrid-cell:focus": {
                                         outline: "none"
                                     },
                                     "& .MuiDataGrid-columnHeaderTitle": {
                                         fontWeight: "bold"
                                     }
                                 },
-                                rows: null !== (v = null == I ? void 0 : I.otherRuns) && void 0 !== v ? v : [],
+                                rows: null !== (d = null == j ? void 0 : j.otherRuns) && void 0 !== d ? d : [],
                                 disableColumnMenu: !0,
                                 rowsPerPageOptions: [5],
                                 columns: [{
                                     field: "runId",
                                     headerName: "runId",
                                     width: 1,
                                     editable: !1,
@@ -725,15 +731,15 @@
                                         children: "Status"
                                     }), (0, i.jsx)(b.Z, {
                                         value: N,
                                         children: "Date"
                                     })]
                                 })]
                             }), (0, i.jsx)(x.Z, {
-                                children: (0, i.jsx)(j.Z, {
+                                children: (0, i.jsx)(k.Z, {
                                     size: "small",
                                     InputLabelProps: {
                                         shrink: !0
                                     },
                                     label: "Search",
                                     onChange: function(t) {
                                         var e, n = t.target.value;
@@ -745,15 +751,15 @@
                                         i.trim() && P(i)
                                     },
                                     value: D,
                                     onKeyDown: function(t) {
                                         "Enter" === t.key && D && tt(D)
                                     },
                                     InputProps: {
-                                        endAdornment: (0, i.jsx)(k.Z, {
+                                        endAdornment: (0, i.jsx)(j.Z, {
                                             position: "end",
                                             children: (0, i.jsx)(p.Z, {
                                                 children: (0, i.jsx)(d.Z, {})
                                             })
                                         })
                                     },
                                     inputProps: {
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/group/[groupName].html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/groups.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/groups.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/role/[roleName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/role/[roleName].html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/connections.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/roles.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/user/[userName].html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/user/[userName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/admin/users.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/users.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/connections.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/tasks.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/index.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/admin/roles.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/query.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/query-f3c47b8d51f1458e.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-44302760e55a8032.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/search.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/query.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/search-e03b34f74065bab5.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/query-f3c47b8d51f1458e.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/base_logo.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/base_logo.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/clearIcon.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/clearIcon.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/creature.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/creature.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/favicon.ico` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/logo192.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/logo512.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/static/welcomebackground.png` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/static/welcomebackground.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/dashboard/out/tasks.html` & `featureform_enterprise-0.13.2rc0/src/featureform/dashboard/out/404.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-ff28ddf757476fd7.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-31dc8fc1d5040dae.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js" defer=""></script><script src="/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d61fafb974c05741.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js" defer=""></script><script src="/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"-bfbor4dtq4HuL8LA_NPy","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"IC-T5dqiUn3tRG10EsGwe","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/deploy.py` & `featureform_enterprise-0.13.2rc0/src/featureform/deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/enums.py` & `featureform_enterprise-0.13.2rc0/src/featureform/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 class FilePrefix(Enum):
     S3 = ("s3://", "s3a://")
     S3A = ("s3a://",)
     HDFS = ("hdfs://",)
     GCS = ("gs://",)
     AZURE = ("abfss://",)
+    GLUE = ("glue://",)
 
     def __init__(self, *valid_prefixes):
         self.prefixes = valid_prefixes
 
     @property
     def value(self):
         return self.prefixes[0]
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/exceptions.py` & `featureform_enterprise-0.13.2rc0/src/featureform/exceptions.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/format.py` & `featureform_enterprise-0.13.2rc0/src/featureform/format.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/get.py` & `featureform_enterprise-0.13.2rc0/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/grpc_client.py` & `featureform_enterprise-0.13.2rc0/src/featureform/grpc_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/lib/auth.py` & `featureform_enterprise-0.13.2rc0/src/featureform/lib/auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/list.py` & `featureform_enterprise-0.13.2rc0/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/proto/metadata.proto` & `featureform_enterprise-0.13.2rc0/src/featureform/proto/metadata.proto`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,16 @@
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 14;
     Tags tags = 15;
     Properties properties = 16;
     ComputationMode mode = 18;
     bool is_embedding = 19;
     int32 dimension = 20;
-    string task_id = 23;
+    string task_id = 23 [deprecated=true];
+    repeated string task_id_list = 24;
     FeatureParameters additional_parameters = 22;
 }
 
 message FeatureParameters {
     oneof feature_type {
         PrecomputedFeatureParameters precomputed = 1;
         OndemandFeatureParameters ondemand = 2;
@@ -292,15 +293,16 @@
     repeated NameVariant trainingsets = 11;
     oneof location {
         Columns columns = 12;
         Stream stream = 16;
     }
     Tags tags = 13;
     Properties properties = 14;
-    string task_id = 15;
+    string task_id = 15 [deprecated=true];
+    repeated string task_id_list = 17;
 }
 
 message Provider {
     string name = 1;
     string description = 2;
     string type = 3;
     string software = 4;
@@ -333,15 +335,16 @@
     repeated NameVariant features = 8;
     NameVariant label = 9;
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 14;
     repeated FeatureLag feature_lags = 15;
     Tags tags = 16;
     Properties properties = 17;
-    string task_id = 18;
+    string task_id = 18 [deprecated=true];
+    repeated string task_id_list = 19;
 }
 
 message Entity {
     string name = 1;
     string description = 2;
     ResourceStatus status = 3;
     repeated NameVariant features = 4;
@@ -395,16 +398,17 @@
     repeated NameVariant trainingsets = 10;
     repeated NameVariant features = 11;
     repeated NameVariant labels = 12;
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 16;
     Tags tags = 17;
     Properties properties = 18;
-    string task_id = 19;
+    string task_id = 19 [deprecated=true];
     google.protobuf.Duration max_job_duration = 20;
+    repeated string task_id_list = 21;
 }
 
 message Transformation {
     oneof type {
         SQLTransformation SQLTransformation= 1;
         DFTransformation DFTransformation= 2;
     }
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/proto/serving.proto` & `featureform_enterprise-0.13.2rc0/src/featureform/proto/serving.proto`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 option go_package = "github.com/featureform/proto";
 
 package featureform.serving.proto;
 
 service Feature {
   rpc TrainingData(TrainingDataRequest) returns (stream TrainingDataRow) {}
-  rpc TrainingTestSplit(stream TrainingTestSplitRequest) returns (stream TrainingTestSplitResponse) {}
+  rpc TrainTestSplit(stream TrainTestSplitRequest) returns (stream BatchTrainTestSplitResponse) {}
   rpc TrainingDataColumns(TrainingDataColumnsRequest) returns (TrainingColumns) {}
   rpc FeatureServe(FeatureServeRequest) returns (FeatureRow) {}
   rpc SourceData(SourceDataRequest) returns (stream SourceDataRow) {}
   rpc SourceColumns(SourceColumnRequest) returns (SourceDataColumns) {}
   rpc Nearest(NearestRequest) returns (NearestResponse) {}
   rpc BatchFeatureServe(BatchFeatureServeRequest) returns (stream BatchFeatureRow) {}
   rpc GetResourceLocation(ResourceIdRequest) returns (ResourceLocation) {}
@@ -36,67 +36,67 @@
 
 message TrainingDataRow {
   repeated Value features = 1;
   Value label = 2;
 }
 
 message FeatureServeRequest {
-    repeated FeatureID features = 1;
-    repeated Entity entities = 2;
-    Model model = 3;
+  repeated FeatureID features = 1;
+  repeated Entity entities = 2;
+  Model model = 3;
 }
 
 message FeatureRow {
   // Deprecated: Use `value_lists` instead.
-  repeated Value values = 1 [deprecated=true];
+  repeated Value values = 1 [deprecated = true];
 
   repeated ValueList value_lists = 2;
 }
 
 message ValueList {
   repeated Value values = 1;
 }
 
 message BatchFeatureServeRequest {
-    repeated FeatureID features = 1;
+  repeated FeatureID features = 1;
 }
 
 message BatchFeatureRow {
-    Value entity = 1;
-    repeated Value features = 2;
+  Value entity = 1;
+  repeated Value features = 2;
 }
 
 message FeatureID {
-    string name = 1;
-    string version = 2;
+  string name = 1;
+  string version = 2;
 }
 
 message Entity {
   string name = 1;
 
   // Deprecated: Use `values` instead.
-  string value = 2 [deprecated=true];
+  string value = 2 [deprecated = true];
 
   repeated string values = 3;
 }
 
 message Value {
-    oneof value {
-        string str_value = 1;
-        int32 int_value = 2;
-        float float_value = 3;
-        double double_value = 4;
-        int64  int64_value = 5;
-        int32  int32_value = 6;
-        bool   bool_value = 7;
-        bytes on_demand_function = 8;
-        Vector32 vector32_value = 9;
-        uint32  uint32_value = 10;
-        uint64  uint64_value = 11;
-    }
+  oneof value {
+    string str_value = 1;
+    int32 int_value = 2;
+    float float_value = 3;
+    double double_value = 4;
+    int64  int64_value = 5;
+    int32  int32_value = 6;
+    bool   bool_value = 7;
+    bytes on_demand_function = 8;
+    Vector32 vector32_value = 9;
+    uint32  uint32_value = 10;
+    uint64  uint64_value = 11;
+  }
 }
 
 message SourceID {
   string name = 1;
   string version = 2;
 }
 
@@ -146,31 +146,36 @@
   int32 type = 3;
 }
 
 message ResourceLocation {
   string location = 1;
 }
 
-message TrainingTestSplitRequest {
+message TrainTestSplitRequest {
   TrainingDataID id = 1;
   Model model = 2;
   float test_size = 3;
   float train_size = 4;
   bool shuffle = 5;
-  int32 random_state = 6;  // Seed for shuffling, if shuffle is true
-  RequestType request_type = 7;  // NEW: Specify the type of data being requested
+  int32 random_state = 6;
+  RequestType request_type = 7;
+  int32 batch_size = 8;
 }
 
 enum RequestType {
   INITIALIZE = 0;
   TRAINING = 1;  // Client is requesting training data
   TEST = 2;      // Client is requesting test data
 }
 
-message TrainingTestSplitResponse {
+message BatchTrainTestSplitResponse {
   RequestType request_type = 1;
   bool iterator_done = 2;
-  oneof training_test_split {
+  oneof result {
     bool initialized = 3;
-    TrainingDataRow row = 4;
+    TrainingDataRows data = 4;
   }
 }
+
+message TrainingDataRows {
+  repeated TrainingDataRow rows = 1;
+}
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/register.py` & `featureform_enterprise-0.13.2rc0/src/featureform/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 NameVariant = Tuple[str, str]
 
 s3_config = S3StoreConfig("", "", AWSStaticCredentials("id", "secret"))
 NON_INFERENCE_STORES = [s3_config.type()]
 
 
 def set_tags_properties(tags: Optional[List[str]], properties: Optional[dict]):
+    """
+    Helper function to set default values for tags and properties
+    """
     if tags is None:
         tags = []
     if properties is None:
         properties = {}
     return tags, properties
 
 
@@ -193,14 +196,65 @@
 
 class OfflineSparkProvider(OfflineProvider):
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
+    def register_iceberg_table(
+        self,
+        name: str,
+        database: str,
+        table: str,
+        variant: str = "",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        tags: Optional[List[str]] = None,
+        properties: Optional[dict] = None,
+    ):
+        """
+        Register an Iceberg table as a primary data source.
+
+        **Examples**
+
+        ```
+        spark = client.get_provider("my_spark")
+        transactions = spark.register_iceberg_table(
+            name="transactions",
+            database="fraud",
+            table="transactions",
+            description="A dataset of fraudulent transactions"
+        )
+        ```
+
+        Args:
+            name (str): Name of table to be registered
+            database (str): Name of database
+            table (str): Name of table
+            variant (str): Name of variant to be registered
+            owner (Union[str, UserRegistrar]): Owner
+            description (str): Description of table to be registered
+            tags (List[str]): Tags
+            properties (dict): Properties
+        Returns:
+            source (ColumnSourceRegistrar): source
+        """
+        tags, properties = set_tags_properties(tags, properties)
+
+        return self.__registrar.register_primary_data(
+            name=name,
+            variant=variant,
+            location=IcebergTable(database, table),
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
+
     def register_file(
         self,
         name: str,
         file_path: str,
         variant: str = "",
         owner: Union[str, UserRegistrar] = "",
         description: str = "",
@@ -232,15 +286,15 @@
             source (ColumnSourceRegistrar): source
         """
         FilePrefix.validate(self.__provider.config.store_type, file_path)
 
         return self.__registrar.register_primary_data(
             name=name,
             variant=variant,
-            location=SQLTable(file_path),
+            location=FileStore(file_path),
             owner=owner,
             provider=self.name(),
             description=description,
             tags=tags,
             properties=properties,
         )
 
@@ -1352,15 +1406,15 @@
         if not include_columns_set.issubset(all_columns_set):
             raise ValueError(
                 f"{all_columns_set - include_columns_set} columns are not in the dataframe"
             )
 
         if not exclude_columns_set.issubset(all_columns_set):
             raise ValueError(
-                f"{all_columns_set - exclude_columns_set} columns are not in the dataframe"
+                f"Exclude columns: {exclude_columns_set - all_columns_set} columns are not in the dataframe"
             )
 
         if not include_columns_set.isdisjoint(exclude_columns_set):
             raise ValueError(
                 f"{include_columns_set.intersection(exclude_columns_set)} cannot be in the include and exclude lists"
             )
 
@@ -3328,14 +3382,15 @@
         return OfflineSQLProvider(self, provider)
 
     def register_spark(
         self,
         name: str,
         executor: ExecutorCredentials,
         filestore: FileStoreProvider,
+        catalog: Optional[Catalog] = None,
         description: str = "",
         team: str = "",
         tags: List[str] = [],
         properties: dict = {},
     ):
         """Register a Spark on Executor provider.
 
@@ -3350,28 +3405,30 @@
         )
         ```
 
         Args:
             name (str): (Immutable) Name of Spark provider to be registered
             executor (ExecutorCredentials): (Mutable) An Executor Provider used for the compute power
             filestore (FileStoreProvider): (Mutable) A FileStoreProvider used for storage of data
+            catalog (Optional[Catalog]): (Mutable) A Catalog Provider used for metadata storage
             description (str): (Mutable) Description of Spark provider to be registered
             team (str): (Mutable) Name of team
             tags (List[str]): (Mutable) Optional grouping mechanism for resources
             properties (dict): (Mutable) Optional grouping mechanism for resources
 
         Returns:
             spark (OfflineSparkProvider): Provider
         """
         tags, properties = set_tags_properties(tags, properties)
         config = SparkConfig(
             executor_type=executor.type(),
             executor_config=executor.config(),
             store_type=filestore.store_type(),
             store_config=filestore.config(),
+            catalog=catalog.config() if catalog is not None else None,
         )
 
         provider = Provider(
             name=name,
             function="OFFLINE",
             description=description,
             team=team,
@@ -4273,14 +4330,15 @@
             schedule=schedule,
             label=label,
             features=processed_features,
             feature_lags=feature_lags,
             tags=tags,
             properties=properties,
         )
+        self.map_client_object_to_resource(resource, resource)
         self.__resources.append(resource)
         return resource
 
     def register_model(
         self, name: str, tags: List[str] = [], properties: dict = {}
     ) -> Model:
         """Register a model.
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/resources.py` & `featureform_enterprise-0.13.2rc0/src/featureform/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1006,35 +1006,57 @@
             return False
         return (
             self.project_id == __value.project_id
             and self.dataset_id == __value.dataset_id
         )
 
 
+class Catalog(ABC):
+    @abstractmethod
+    def config(self):
+        pass
+
+
+@typechecked
+@dataclass
+class GlueCatalog(Catalog):
+    warehouse: str
+
+    def config(self):
+        return {
+            "Warehouse": self.warehouse,
+        }
+
+
 @typechecked
 @dataclass
 class SparkConfig:
     executor_type: str
     executor_config: dict
     store_type: str
     store_config: dict
+    catalog: Optional[dict] = None
 
     def software(self) -> str:
         return "spark"
 
     def type(self) -> str:
         return "SPARK_OFFLINE"
 
     def serialize(self) -> bytes:
         config = {
             "ExecutorType": self.executor_type,
             "StoreType": self.store_type,
             "ExecutorConfig": self.executor_config,
             "StoreConfig": self.store_config,
         }
+
+        if self.catalog is not None:
+            config["Catalog"] = self.catalog
+
         return bytes(json.dumps(config), "utf-8")
 
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, SparkConfig):
             return False
         return (
             self.executor_type == __value.executor_type
@@ -1311,27 +1333,62 @@
             "name": self.name,
             "status": self.status,
             "tags": self.tags,
             "properties": self.properties,
         }
 
 
+class Location(ABC):
+    def path(self):
+        """
+        Return the location of the resource.
+        :return:
+        """
+        raise NotImplementedError
+
+
 @typechecked
 @dataclass
-class SQLTable:
+class SQLTable(Location):
     name: str
 
+    def path(self):
+        return self.name
+
 
 @typechecked
 @dataclass
-class Directory:
-    path: str
+class FileStore(Location):
+    """
+    Contains the location of a path in a cloud file store (S3, GCS, Azure)
+    """
+
+    path_uri: str
+
+    def path(self):
+        return self.path_uri
+
+
+@typechecked
+@dataclass
+class IcebergTable(Location):
+    database: str
+    table: str
 
+    def path(self):
+        return f"glue://{self.database}/{self.table}"
+
+
+@typechecked
+@dataclass
+class Directory(Location):
+    path: str
 
-Location = Union[SQLTable, Directory]
+    def path(self):
+        return self.path
 
 
 class ResourceVariant(ABC):
     name: str
     variant: str
     server_status: ServerStatus
 
@@ -1351,24 +1408,21 @@
 class PrimaryData:
     location: Location
 
     def kwargs(self):
         return {
             "primaryData": pb.PrimaryData(
                 table=pb.PrimarySQLTable(
-                    name=self.location.name,
+                    name=self.location.path(),
                 ),
             ),
         }
 
-    def name(self):
-        return self.location.name
-
     def path(self):
-        return self.location.path
+        return self.location.path()
 
 
 class Transformation:
     pass
 
 
 @typechecked
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/search.py` & `featureform_enterprise-0.13.2rc0/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/serving.py` & `featureform_enterprise-0.13.2rc0/src/featureform/serving.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import inspect
-import math
 import os
-import queue
 import random
 import types
 import warnings
 from collections.abc import Iterator
-from typing import List, Union
+from typing import List, Optional, Union
 
 import dill
+import math
 import numpy as np
 import pandas as pd
-
 from featureform.proto import serving_pb2, serving_pb2_grpc
+from . import GrpcClient, Model, TrainingSetVariant
 from .enums import FileFormat, ResourceType
-from .grpc_client import GrpcClient
 from .register import FeatureColumnResource
-from .resources import Model, TrainingSetVariant
 from .tls import insecure_channel, secure_channel
+
+from .train_test_split import TrainTestSplit
 from .version import check_up_to_date
+from .grpc_client import GrpcClient
 
 
 def check_feature_type(features):
     checked_features = []
     for feature in features:
         if isinstance(feature, tuple):
             checked_features.append(feature)
@@ -104,36 +104,19 @@
         Args:
             name (str): Name of training set to be retrieved
             variant (str): Variant of training set to be retrieved
 
         Returns:
             training_set (Dataset): A training set iterator
         """
-        print(type(name))
         if isinstance(name, TrainingSetVariant):
             variant = name.variant
             name = name.name
         return self.impl.training_set(name, variant, include_label_timestamp, model)
 
-    def train_test_split(self, name, variant="", model: Union[str, Model] = None):
-        """Split the dataset into a training set and a test set.
-
-        Args:
-            name (str): The name of the training set
-            variation (str): The variation of the training set
-            model (Union[str, Model]): The model to use for the training set
-
-        Returns:
-            train_set (Dataset): The training set
-            test_set (Dataset): The test set
-            :param variant:
-        """
-        train, test = self.impl.training_set_test_split(name, variant, model)
-        return train, test
-
     def features(
         self, features, entities, model: Union[str, Model] = None, params: list = None
     ):
         """Returns the feature values for the specified entities.
 
         **Examples**:
         ``` py
@@ -198,20 +181,14 @@
     @staticmethod
     def _create_channel(host, insecure, cert_path):
         if insecure:
             return insecure_channel(host)
         else:
             return secure_channel(host, cert_path)
 
-    # def _create_async_channel(self, host, insecure, cert_path):
-    #     if insecure:
-    #         return async_insecure_channel(host)
-    #     else:
-    #         return secure_channel(host, cert_path)
-
     def training_set(
         self, name, variation, include_label_timestamp, model: Union[str, Model] = None
     ):
         training_set_stream = TrainingSetStream(self._stub, name, variation, model)
         return Dataset(training_set_stream)
 
     def features(
@@ -439,187 +416,14 @@
             except StopIteration:
                 if len(rows) == 0:
                     raise
                 return rows
         return rows
 
 
-class TrainingSetSplitIterator:
-    def __init__(
-        self,
-        req_queue: queue.Queue,
-        resp_queue: queue.Queue,
-        resp_stream,
-        request_type,
-        name,
-        version,
-        test_size,
-        train_size,
-        shuffle,
-        random_state,
-        batch_size,
-        model: Union[str, Model] = None,
-    ):
-        self.name = name
-        self.version = version
-        self.model = model
-        self.test_size = test_size
-        self.train_size = train_size
-        self.shuffle = shuffle
-        self.batch_size = batch_size
-        self.random_state = random_state
-        self.resp_stream = resp_stream
-        self.complete = False
-
-        self.req_queue = req_queue
-        self.resp_queue = resp_queue
-        self._request_type = request_type
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if self.complete:
-            raise StopIteration
-        i = 0
-        batch_features = None
-        batch_label = None
-        while i < self.batch_size:
-            req = serving_pb2.TrainingTestSplitRequest()
-            req.id.name = self.name
-            req.id.version = self.version
-
-            if self.model is not None:
-                req.model.name = (
-                    self.model if isinstance(self.model, str) else self.model.name
-                )
-            req.test_size = self.test_size
-            req.train_size = self.train_size
-            req.shuffle = self.shuffle
-            req.random_state = self.random_state
-            req.request_type = self._request_type
-
-            self.req_queue.put(req)
-
-            next_row = next(self.resp_stream)
-
-            if next_row.iterator_done:
-                self.complete = True
-                if batch_features is None:
-                    raise StopIteration
-                return batch_features, batch_label
-
-            if batch_features is None:
-                row = Row(next_row.row)
-                batch_features = np.array(row.features())
-                batch_label = np.array(row.label())
-            else:
-                batch_features = np.append(
-                    batch_features, Row(next_row.row).features(), axis=0
-                )
-                batch_label = np.append(batch_label, Row(next_row.row).label(), axis=0)
-            i += 1
-
-        return batch_features, batch_label
-
-
-class TrainingSetTestSplit:
-    """
-    Returns two iterators, one for the training set and one for the test set, in that order
-    """
-
-    def __init__(
-        self,
-        stub,
-        name: str,
-        version: str,
-        test_size: float,
-        train_size: float,
-        shuffle: bool,
-        random_state: int,
-        batch_size: int,
-        model: Union[str, Model] = None,
-    ):
-        self.name = name
-        self.version = version
-        self.shuffle = shuffle
-        self.random_state = random_state
-        self.model = model
-        self.test_size = test_size
-        self.train_size = train_size
-        self.batch_size = batch_size
-        self.train_iter = None
-        self.test_iter = None
-        self._stream = None
-        self.stub = stub
-
-        self.req_queue = queue.Queue()
-
-        # initialize the request queue
-        req = serving_pb2.TrainingTestSplitRequest()
-        req.id.name = self.name
-        req.id.version = self.version
-        if self.model is not None:
-            req.model.name = (
-                self.model if isinstance(self.model, str) else self.model.name
-            )
-        req.request_type = serving_pb2.RequestType.INITIALIZE
-        req.test_size = self.test_size
-        req.shuffle = self.shuffle
-        req.random_state = self.random_state
-
-        self.req_queue.put(req)
-
-        self.resp_queue = queue.Queue()
-
-    def request_generator(self):
-        while True:
-            if not self.req_queue.empty():
-                request = self.req_queue.get()
-                yield request
-
-    def split(self):
-        response_stream = self.stub.TrainingTestSplit(self.request_generator())
-        # verify initialization response # TODO: don't think we need this
-        init_response = next(response_stream)
-        if not init_response.initialized:
-            raise ValueError("Failed to initialize training test split")
-
-        self.train_iter = TrainingSetSplitIterator(
-            req_queue=self.req_queue,
-            resp_queue=self.resp_queue,
-            resp_stream=response_stream,
-            request_type=serving_pb2.RequestType.TRAINING,
-            name=self.name,
-            version=self.version,
-            model=self.model,
-            test_size=self.test_size,
-            train_size=self.train_size,
-            shuffle=self.shuffle,
-            random_state=self.random_state,
-            batch_size=self.batch_size,
-        )
-        self.test_iter = TrainingSetSplitIterator(
-            req_queue=self.req_queue,
-            resp_queue=self.resp_queue,
-            resp_stream=response_stream,
-            request_type=serving_pb2.RequestType.TEST,
-            name=self.name,
-            version=self.version,
-            model=self.model,
-            test_size=self.test_size,
-            train_size=self.train_size,
-            shuffle=self.shuffle,
-            random_state=self.random_state,
-            batch_size=self.batch_size,
-        )
-
-        return self.train_iter, self.test_iter
-
-
 class Dataset:
     def __init__(self, stream, dataframe=None):
         """Repeats the Dataset for the specified number of times
 
         Args:
             stream (Iterator): An iterable object.
 
@@ -630,22 +434,22 @@
         self._dataframe = dataframe
 
     def train_test_split(
         self,
         test_size: float = 0,
         train_size: float = 0,
         shuffle: bool = True,
-        random_state: Union[int, None] = None,
+        random_state: Optional[int] = None,
         batch_size: int = 1,
     ):
         """
         (This functionality is currently only available for Clickhouse).
 
         Splits an existing training set into training and testing iterators. The split is processed on the underlying
-        provider and calculated and serving time.
+        provider and calculated at serving time.
 
         **Examples**:
 
         ``` py
         import featureform as ff
         client = ff.Client()
         train, test = client
@@ -696,65 +500,68 @@
 
         Args:
             test_size (float): The ratio of test set size to train set size. Must be a value between 0 and 1. If excluded
                 it will be the complement to the train_size. One of test_size or train_size must be specified.
             train_size (float): The ratio of train set size to train set size. Must be a value between 0 and 1. If excluded
                 it will be the complement to the test_size. One of test_size or train_size must be specified.
             shuffle (bool): Whether to shuffle the dataset before splitting.
-            random_state (Union[int, None]): A random state to shuffle the dataset. If None, the dataset will be shuffled
+            random_state (Optional[int]): A random state to shuffle the dataset. If None, the dataset will be shuffled
                 randomly on every call. If >0, the value will be used a seed to create random shuffle that can be repeated
                 if subsequent calls use the same seed.
             batch_size (int): The size of the batch to return from the iterator. Must be greater than 0.
 
         Returns:
             train (Iterator): An iterator for training values.
             test (Iterator): An iterator for testing values.
         """
         if batch_size < 1:
             raise ValueError("batch_size must be 1 or greater")
 
-        if random_state == 0:
-            raise ValueError("random_state must be greater than zero or None")
+        if random_state is not None and random_state < 0:
+            raise ValueError("random_state must be 0 or greater")
 
         test_size, train_size = self.validate_test_size(test_size, train_size)
 
         name = self._stream.name
         variant = self._stream.version
         stub = self._stream._stub
         model = self._stream.model if hasattr(self._stream, "model") else None
-        if random_state is None:
-            random_state = 0
 
-        train, test = TrainingSetTestSplit(
+        train, test = TrainTestSplit(
             stub=stub,
             name=name,
             version=variant,
             model=model,
             test_size=test_size,
             train_size=train_size,
             shuffle=shuffle,
-            random_state=random_state,
+            random_state=(0 if random_state is None else random_state),
             batch_size=batch_size,
         ).split()
 
         return train, test
 
     @staticmethod
     def validate_test_size(test_size, train_size):
-        if test_size > 1 or test_size < 0:
+        # Validate ranges
+        if not 0 <= test_size <= 1:
             raise ValueError("test_size must be between 0 and 1")
-        if train_size > 1 or train_size < 0:
+        if not 0 <= train_size <= 1:
             raise ValueError("train_size must be between 0 and 1")
-        if test_size != 0 and train_size != 0:
-            if test_size + train_size != 1:
-                raise ValueError("test_size + train_size must equal 1")
-        if test_size == 0 and train_size != 0:
+
+        # If both are specified but don't sum to 1, it's an error
+        if test_size != 0 and train_size != 0 and test_size + train_size != 1:
+            raise ValueError("test_size + train_size must equal 1 if both are non-zero")
+
+        # Auto-adjust if one is 0
+        if test_size == 0 and train_size > 0:
             test_size = 1 - train_size
-        if test_size != 0 and train_size == 0:
+        elif train_size == 0 and test_size > 0:
             train_size = 1 - test_size
+
         return test_size, train_size
 
     def dataframe(self, spark_session=None):
         """Returns the training set as a Pandas DataFrame or Spark DataFrame.
         Args:
         - spark_session: Optional(SparkSession)
 
@@ -952,15 +759,15 @@
     def __next__(self):
         next_val = next(self._stream)
         return next_val
 
 
 class Row:
     def __init__(self, proto_row):
-        self._types = [parse_proto_type(feature) for feature in proto_row.features]
+        self._types = [proto_type_to_np_type(feature) for feature in proto_row.features]
         self._features = np.array(
             [parse_proto_value(feature) for feature in proto_row.features],
             dtype=get_numpy_array_type(self._types),
         )
         self._label = parse_proto_value(proto_row.label)
         self._row = np.append(self._features, self._label)
 
@@ -1035,15 +842,15 @@
 
 
 def parse_proto_value(value):
     """parse_proto_value is used to parse the one of Value message"""
     return getattr(value, value.WhichOneof("value"))
 
 
-def parse_proto_type(value):
+def proto_type_to_np_type(value):
     type_mapping = {
         "str_value": str,
         "int_value": np.int32,
         "int32_value": np.int32,
         "int64_value": np.int64,
         "float_value": np.float32,
         "double_value": np.float64,
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform/status_display.py` & `featureform_enterprise-0.13.2rc0/src/featureform/status_display.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/tls.py` & `featureform_enterprise-0.13.2rc0/src/featureform/tls.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/type_objects.py` & `featureform_enterprise-0.13.2rc0/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/variant_names_generator.py` & `featureform_enterprise-0.13.2rc0/src/featureform/variant_names_generator.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform/version.py` & `featureform_enterprise-0.13.2rc0/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/PKG-INFO` & `featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.0rc0
+Version: 0.13.2rc0
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13rc0/src/featureform_enterprise.egg-info/SOURCES.txt` & `featureform_enterprise-0.13.2rc0/src/featureform_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 src/featureform/parse.py
 src/featureform/register.py
 src/featureform/resources.py
 src/featureform/search.py
 src/featureform/serving.py
 src/featureform/status_display.py
 src/featureform/tls.py
+src/featureform/train_test_split.py
 src/featureform/type_objects.py
 src/featureform/types.py
 src/featureform/variant_names_generator.py
 src/featureform/version.py
 src/featureform/dashboard/out/404.html
 src/featureform/dashboard/out/[type].html
 src/featureform/dashboard/out/connections.html
 src/featureform/dashboard/out/index.html
 src/featureform/dashboard/out/query.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/tasks.html
 src/featureform/dashboard/out/[type]/[entity].html
-src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/_buildManifest.js
-src/featureform/dashboard/out/_next/static/-bfbor4dtq4HuL8LA_NPy/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/_buildManifest.js
+src/featureform/dashboard/out/_next/static/IC-T5dqiUn3tRG10EsGwe/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
 src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
 src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
 src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
@@ -271,21 +272,21 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
 src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
 src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
-src/featureform/dashboard/out/_next/static/chunks/pages/_app-ff28ddf757476fd7.js
+src/featureform/dashboard/out/_next/static/chunks/pages/_app-d61fafb974c05741.js
 src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
 src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
 src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
 src/featureform/dashboard/out/_next/static/chunks/pages/query-f3c47b8d51f1458e.js
 src/featureform/dashboard/out/_next/static/chunks/pages/search-e03b34f74065bab5.js
-src/featureform/dashboard/out/_next/static/chunks/pages/tasks-31dc8fc1d5040dae.js
+src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
```

### Comparing `featureform_enterprise-0.13rc0/tests/test_auth.py` & `featureform_enterprise-0.13.2rc0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_autogenerated_variants.py` & `featureform_enterprise-0.13.2rc0/tests/test_autogenerated_variants.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_class_api.py` & `featureform_enterprise-0.13.2rc0/tests/test_class_api.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_cli.py` & `featureform_enterprise-0.13.2rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_client.py` & `featureform_enterprise-0.13.2rc0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-import csv
-import os
-import shutil
-import stat
 import sys
-import time
-from tempfile import NamedTemporaryFile
-from unittest import TestCase
-from unittest import mock
-
-import numpy as np
-import pandas as pd
-import pytest
 
 sys.path.insert(0, "client/src/")
-from featureform import Client
-import serving_cases as cases
 import featureform as ff
-from featureform.serving import check_feature_type, Row, Dataset
-from featureform.enums import ResourceType
 from featureform.resources import (
     PostgresConfig,
     RedshiftConfig,
     ClickHouseConfig,
     GCPCredentials,
     BigQueryConfig,
     CassandraConfig,
```

### Comparing `featureform_enterprise-0.13rc0/tests/test_deploy.py` & `featureform_enterprise-0.13.2rc0/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_enums.py` & `featureform_enterprise-0.13.2rc0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_executor_resources.py` & `featureform_enterprise-0.13.2rc0/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_getting_model.py` & `featureform_enterprise-0.13.2rc0/tests/test_getting_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_multi_feature.py` & `featureform_enterprise-0.13.2rc0/tests/test_multi_feature.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_ondemand_features.py` & `featureform_enterprise-0.13.2rc0/tests/test_ondemand_features.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_parse.py` & `featureform_enterprise-0.13.2rc0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_resource_registration.py` & `featureform_enterprise-0.13.2rc0/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_search.py` & `featureform_enterprise-0.13.2rc0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_serving_model.py` & `featureform_enterprise-0.13.2rc0/tests/test_serving_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_source_columns.py` & `featureform_enterprise-0.13.2rc0/tests/test_source_columns.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_source_dataframe.py` & `featureform_enterprise-0.13.2rc0/tests/test_source_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_spark_provider.py` & `featureform_enterprise-0.13.2rc0/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_tags_and_properties.py` & `featureform_enterprise-0.13.2rc0/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_train_test_split.py` & `featureform_enterprise-0.13.2rc0/tests/test_train_test_split.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,87 @@
-import featureform as ff
-from featureform.serving import Dataset
 import os
-from featureform.proto import serving_pb2
+
 import numpy as np
 import pytest
-import time
+
+from featureform.proto import serving_pb2
+from featureform.serving import Dataset
 
 real_path = os.path.realpath(__file__)
 dir_path = os.path.dirname(real_path)
 
 
-def response(req_type, iterator_done):
-    if req_type == 0:
-        request_type = serving_pb2.RequestType.INITIALIZE
-        return serving_pb2.TrainingTestSplitResponse(
-            request_type=request_type, initialized=True
+def response(
+    req_type, iterator_done, batch_size
+) -> serving_pb2.BatchTrainTestSplitResponse:
+    if req_type == serving_pb2.RequestType.INITIALIZE:
+        return serving_pb2.BatchTrainTestSplitResponse(
+            request_type=req_type, initialized=True
         )
-    elif req_type == 1:
-        request_type = serving_pb2.RequestType.TRAINING
+    elif req_type == serving_pb2.RequestType.TRAINING:
         label_value = "train"
-    elif req_type == 2:
-        request_type = serving_pb2.RequestType.TEST
+    elif req_type == serving_pb2.RequestType.TEST:
         label_value = "test"
 
-    req = serving_pb2.TrainingTestSplitResponse(
-        request_type=request_type,
-        row=serving_pb2.TrainingDataRow(
-            features=[
-                serving_pb2.Value(str_value="f1"),
-                serving_pb2.Value(int_value=1),
-                serving_pb2.Value(bool_value=False),
-            ],
-            label=serving_pb2.Value(str_value=label_value),
-        ),
-        iterator_done=iterator_done,
+    row = serving_pb2.TrainingDataRow(
+        features=[
+            serving_pb2.Value(str_value="f1"),
+            serving_pb2.Value(int_value=1),
+            serving_pb2.Value(bool_value=False),
+        ],
+        label=serving_pb2.Value(str_value=label_value),
     )
 
-    # training_data = serving_pb2.TrainingDataRow()
-    # req.row = training_data
-
-    return req
+    return serving_pb2.BatchTrainTestSplitResponse(
+        request_type=req_type,
+        data=serving_pb2.TrainingDataRows(rows=[row] * batch_size),
+        iterator_done=iterator_done,
+    )
 
 
 class MockGrpcStub:
-    def __init__(self, num_rows):
+    def __init__(self, num_rows, batch_size=1):
         self.num_rows = num_rows
         self.train_rows = 0
         self.test_rows = 0
+        self.batch_size = batch_size
 
-    def TrainingTestSplit(self, iterator):
+    def TrainTestSplit(self, iterator) -> serving_pb2.BatchTrainTestSplitResponse:
+        rows_to_return = self.batch_size
         for value in iterator:
             iterator_done = False
-            if value.request_type == 1:
-                self.train_rows += 1
+            if value.request_type == serving_pb2.RequestType.TRAINING:
+                self.train_rows += self.batch_size
 
                 if self.train_rows > self.num_rows:
+                    rows_to_return = self.num_rows - (self.train_rows - self.batch_size)
                     iterator_done = True
-            elif value.request_type == 2:
-                self.test_rows += 1
+            elif value.request_type == serving_pb2.RequestType.TEST:
+                self.test_rows += self.batch_size
 
                 if self.test_rows > self.num_rows:
+                    rows_to_return = self.num_rows - (self.test_rows - self.batch_size)
                     iterator_done = True
-            yield response(value.request_type, iterator_done)
+            yield response(value.request_type, iterator_done, rows_to_return)
 
 
 class MockStream:
     name = None
     version = None
     model = None
     _stub = None
 
-    def __init__(self, name, version, num_rows):
+    def __init__(self, name, version, num_rows, batch_size=1):
         self.name = name
         self.version = version
-        self.num_rows = num_rows
-        self._stub = MockGrpcStub(self.num_rows)
+        self._stub = MockGrpcStub(num_rows, batch_size)
 
 
 @pytest.mark.parametrize(
-    "kwargs,should_fail",
+    "kwargs, should_fail",
     [
         (
             {
                 "test_size": 0.5,
                 "train_size": 0.5,
                 "shuffle": True,
                 "random_state": None,
@@ -146,23 +145,23 @@
 
     for features, label in test:
         assert np.array_equal(features, np.array([["f1", 1, False]], dtype="O"))
         assert np.array_equal(label, np.array(["test"]))
 
 
 def test_train_test_batch():
-    train_test_stream = MockStream("name", "variant", 10)
+    train_test_stream = MockStream("name", "variant", 10, batch_size=5)
     dataset = Dataset(train_test_stream)
     train, test = dataset.train_test_split(
         test_size=0.5, train_size=0.5, shuffle=True, random_state=None, batch_size=5
     )
     i = 0
     for features, label in train:
         if i > 1:
-            break
+            break  # Ensures we only check the first two batches
 
         assert np.array_equal(
             features,
             np.array(
                 [
                     ["f1", 1, False],
                     ["f1", 1, False],
@@ -196,23 +195,23 @@
             ),
         )
         assert np.array_equal(label, np.array(["test", "test", "test", "test", "test"]))
         i += 1
 
 
 def test_train_test_partial_batch():
-    train_test_stream = MockStream("name", "variant", 3)
+    train_test_stream = MockStream("name", "variant", 3, batch_size=5)
     dataset = Dataset(train_test_stream)
     train, test = dataset.train_test_split(
         test_size=0.5, train_size=0.5, shuffle=True, random_state=None, batch_size=5
     )
     i = 0
     for features, label in train:
         if i > 1:
-            break
+            break  # Ensures we only check the first two batches
 
         assert np.array_equal(
             features,
             np.array(
                 [
                     ["f1", 1, False],
                     ["f1", 1, False],
```

### Comparing `featureform_enterprise-0.13rc0/tests/test_training_set_dataframe.py` & `featureform_enterprise-0.13.2rc0/tests/test_training_set_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13rc0/tests/test_updating_provider.py` & `featureform_enterprise-0.13.2rc0/tests/test_updating_provider.py`

 * *Files identical despite different names*

