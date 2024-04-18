# Comparing `tmp/libhmac-python-20240129.tar.gz` & `tmp/libhmac-python-20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libhmac-python-20240129.tar", last modified: Mon Jan 29 06:30:29 2024, max compression
+gzip compressed data, was "libhmac-python-20240417.tar", last modified: Thu Apr 18 01:43:54 2024, max compression
```

## Comparing `libhmac-python-20240129.tar` & `libhmac-python-20240417.tar`

### file list

```diff
@@ -1,586 +1,586 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-29 05:22:13.000000 libhmac-20240129/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-29 05:29:23.000000 libhmac-20240129/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 05:22:13.000000 libhmac-20240129/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2460 2024-01-29 05:29:33.000000 libhmac-20240129/libhmac.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-29 05:29:24.000000 libhmac-20240129/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:27.000000 libhmac-20240129/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:18.000000 libhmac-20240129/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:18.000000 libhmac-20240129/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:18.000000 libhmac-20240129/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:10:18.000000 libhmac-20240129/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:18.000000 libhmac-20240129/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:18.000000 libhmac-20240129/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:10:18.000000 libhmac-20240129/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-29 05:29:19.000000 libhmac-20240129/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-29 05:29:19.000000 libhmac-20240129/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:18.000000 libhmac-20240129/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-29 05:29:19.000000 libhmac-20240129/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:18.000000 libhmac-20240129/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:10:17.000000 libhmac-20240129/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:18.000000 libhmac-20240129/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-29 05:29:19.000000 libhmac-20240129/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:18.000000 libhmac-20240129/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:18.000000 libhmac-20240129/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-29 05:29:19.000000 libhmac-20240129/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:18.000000 libhmac-20240129/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:10:18.000000 libhmac-20240129/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:10:18.000000 libhmac-20240129/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:18.000000 libhmac-20240129/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:10:18.000000 libhmac-20240129/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:27.000000 libhmac-20240129/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2024-01-29 05:22:13.000000 libhmac-20240129/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18774 2024-01-29 05:22:13.000000 libhmac-20240129/include/libhmac.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:27.000000 libhmac-20240129/include/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2024-01-29 05:22:13.000000 libhmac-20240129/include/libhmac/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-01-29 05:29:33.000000 libhmac-20240129/include/libhmac/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5110 2024-01-29 05:22:13.000000 libhmac-20240129/include/libhmac/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4979 2024-01-29 05:29:33.000000 libhmac-20240129/include/libhmac/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-29 05:23:05.000000 libhmac-20240129/include/libhmac/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-01-29 05:22:13.000000 libhmac-20240129/include/libhmac/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-29 05:22:13.000000 libhmac-20240129/include/libhmac/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-29 05:29:33.000000 libhmac-20240129/include/libhmac/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24876 2024-01-29 05:29:23.000000 libhmac-20240129/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18774 2024-01-29 05:29:33.000000 libhmac-20240129/include/libhmac.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-29 05:22:13.000000 libhmac-20240129/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-29 05:22:13.000000 libhmac-20240129/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-29 05:22:13.000000 libhmac-20240129/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-29 05:22:13.000000 libhmac-20240129/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-29 05:22:13.000000 libhmac-20240129/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-29 05:22:13.000000 libhmac-20240129/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-29 05:22:13.000000 libhmac-20240129/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-29 05:22:13.000000 libhmac-20240129/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-29 05:22:13.000000 libhmac-20240129/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-01-29 05:29:33.000000 libhmac-20240129/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14987 2024-01-29 05:29:23.000000 libhmac-20240129/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15866 2024-01-29 05:28:50.000000 libhmac-20240129/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-29 05:22:13.000000 libhmac-20240129/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-29 05:22:13.000000 libhmac-20240129/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-29 05:22:13.000000 libhmac-20240129/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21924 2024-01-29 05:29:23.000000 libhmac-20240129/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26927 2024-01-29 05:29:23.000000 libhmac-20240129/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-01-29 05:29:08.000000 libhmac-20240129/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1571 2023-12-03 09:10:19.000000 libhmac-20240129/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:10:17.000000 libhmac-20240129/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-29 05:29:23.000000 libhmac-20240129/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:27.000000 libhmac-20240129/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/libhmac.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-01-29 05:22:14.000000 libhmac-20240129/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/libhmac-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:27.000000 libhmac-20240129/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2165 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-01-29 05:29:33.000000 libhmac-20240129/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/libhmac-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-01-29 05:22:13.000000 libhmac-20240129/dpkg/libhmac-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-01-29 05:29:33.000000 libhmac-20240129/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-29 05:22:13.000000 libhmac-20240129/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1454144 2024-01-29 05:29:22.000000 libhmac-20240129/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-29 05:29:23.000000 libhmac-20240129/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-29 05:29:23.000000 libhmac-20240129/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmacsum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6731 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmacsum/hmacsum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha256/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/hmac_test_sha256/hmac_test_sha256.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha1_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_sha1_context/hmac_test_sha1_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_md5_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4881 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_md5_context/hmac_test_md5_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1042 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha1/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4860 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/hmac_test_sha1/hmac_test_sha1.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha512_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_sha512_context/hmac_test_sha512_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha512/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/hmac_test_sha512/hmac_test_sha512.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4626 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_support/hmac_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha224_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_sha224_context/hmac_test_sha224_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha256_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_sha256_context/hmac_test_sha256_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_md5/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4857 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/hmac_test_md5/hmac_test_md5.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4620 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/hmac_test_error/hmac_test_error.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17036 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/libhmac.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6796 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/hmac_test_sha224/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-01-29 05:22:53.000000 libhmac-20240129/msvscpp/hmac_test_sha224/hmac_test_sha224.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19934 2024-01-29 05:29:24.000000 libhmac-20240129/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/pyhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6513 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/pyhmac/pyhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:29.000000 libhmac-20240129/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-29 05:22:26.000000 libhmac-20240129/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      197 2024-01-29 05:22:13.000000 libhmac-20240129/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27691 2024-01-29 05:29:23.000000 libhmac-20240129/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-01-29 05:29:07.000000 libhmac-20240129/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      320 2024-01-29 05:22:13.000000 libhmac-20240129/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-29 05:29:23.000000 libhmac-20240129/INSTALL
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      358 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-29 05:22:13.000000 libhmac-20240129/pyproject.toml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/hmactools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_system_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3376 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2023-12-03 09:10:17.000000 libhmac-20240129/hmactools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4142 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4799 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/sum_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8333 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmacsum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38351 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/sum_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28823 2024-01-29 05:29:23.000000 libhmac-20240129/hmactools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1267 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-01-29 05:22:14.000000 libhmac-20240129/hmactools/hmactools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-01-29 05:22:13.000000 libhmac-20240129/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-29 05:29:23.000000 libhmac-20240129/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-29 05:22:13.000000 libhmac-20240129/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2024-01-29 05:23:05.000000 libhmac-20240129/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:10:17.000000 libhmac-20240129/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29781 2024-01-29 05:29:24.000000 libhmac-20240129/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-29 05:29:12.000000 libhmac-20240129/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-29 05:29:24.000000 libhmac-20240129/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26969 2024-01-29 05:29:23.000000 libhmac-20240129/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-01-29 05:29:10.000000 libhmac-20240129/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3043 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 09:10:19.000000 libhmac-20240129/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2024-01-29 05:22:14.000000 libhmac-20240129/manuals/hmacsum.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      152 2023-12-03 09:10:16.000000 libhmac-20240129/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-01-29 05:22:14.000000 libhmac-20240129/manuals/libhmac.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23888 2024-01-29 05:29:24.000000 libhmac-20240129/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27739 2024-01-29 05:22:53.000000 libhmac-20240129/tests/hmac_test_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7073 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_md5.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/tests/input/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/tests/input/public/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/empty
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       64 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test8
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       56 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test7
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test2
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       80 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test6
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       62 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test5
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       26 2023-12-03 09:10:16.000000 libhmac-20240129/tests/input/public/test4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15803 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14435 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14579 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28073 2024-01-29 05:22:53.000000 libhmac-20240129/tests/hmac_test_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4126 2024-01-29 05:22:53.000000 libhmac-20240129/tests/Makefile.am
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5650 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_sha2sum.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4439 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_md5sum.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4069 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28089 2024-01-29 05:22:53.000000 libhmac-20240129/tests/hmac_test_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7018 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28090 2024-01-29 05:22:53.000000 libhmac-20240129/tests/hmac_test_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52137 2024-01-29 05:29:24.000000 libhmac-20240129/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-29 05:22:14.000000 libhmac-20240129/tests/hmac_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27584 2024-01-29 05:22:53.000000 libhmac-20240129/tests/hmac_test_md5_context.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4461 2024-01-29 05:22:14.000000 libhmac-20240129/tests/test_sha1sum.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-29 05:22:14.000000 libhmac-20240129/tests/pyhmac_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4151 2024-01-29 05:23:05.000000 libhmac-20240129/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/sha512_context_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1224 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/sha1_context_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1941 2023-12-03 09:10:20.000000 libhmac-20240129/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/ossfuzz_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1218 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/md5_context_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/sha256_context_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34483 2024-01-29 05:29:24.000000 libhmac-20240129/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-01-29 05:22:13.000000 libhmac-20240129/ossfuzz/sha224_context_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-29 05:29:19.000000 libhmac-20240129/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-01-29 05:29:33.000000 libhmac-20240129/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-12-03 09:10:18.000000 libhmac-20240129/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1100 2024-01-29 05:29:33.000000 libhmac-20240129/libhmac/libhmac.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31285 2024-01-29 05:29:24.000000 libhmac-20240129/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-01-29 05:22:13.000000 libhmac-20240129/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27749 2024-01-29 05:29:23.000000 libhmac-20240129/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-01-29 05:29:11.000000 libhmac-20240129/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:18.000000 libhmac-20240129/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:18.000000 libhmac-20240129/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:18.000000 libhmac-20240129/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:18.000000 libhmac-20240129/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:18.000000 libhmac-20240129/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:18.000000 libhmac-20240129/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:18.000000 libhmac-20240129/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:18.000000 libhmac-20240129/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:18.000000 libhmac-20240129/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-29 05:29:33.000000 libhmac-20240129/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:18.000000 libhmac-20240129/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:18.000000 libhmac-20240129/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50446 2024-01-29 05:29:24.000000 libhmac-20240129/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-01-29 05:29:15.000000 libhmac-20240129/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37247 2024-01-29 05:29:23.000000 libhmac-20240129/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/pyhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1953 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7203 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9771 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1343 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2023-12-03 09:10:20.000000 libhmac-20240129/pyhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1337 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7233 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7909 2024-01-29 05:23:05.000000 libhmac-20240129/pyhmac/pyhmac.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45738 2024-01-29 05:29:24.000000 libhmac-20240129/pyhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9673 2024-01-29 05:22:14.000000 libhmac-20240129/pyhmac/pyhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26803 2024-01-29 05:29:23.000000 libhmac-20240129/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-29 05:29:09.000000 libhmac-20240129/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-29 06:30:28.000000 libhmac-20240129/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-29 05:29:05.000000 libhmac-20240129/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26316 2024-01-29 05:29:23.000000 libhmac-20240129/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56650 2024-01-29 05:29:21.000000 libhmac-20240129/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6264 2024-01-29 05:22:13.000000 libhmac-20240129/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-01-29 06:30:29.590866 libhmac-20240129/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-17 16:22:09.000000 libhmac-20240417/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-17 19:07:45.000000 libhmac-20240417/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:22:09.000000 libhmac-20240417/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2460 2024-04-17 19:08:03.000000 libhmac-20240417/libhmac.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-17 19:07:45.000000 libhmac-20240417/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:50.000000 libhmac-20240417/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:18.000000 libhmac-20240417/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:18.000000 libhmac-20240417/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:18.000000 libhmac-20240417/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:18.000000 libhmac-20240417/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:18.000000 libhmac-20240417/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-17 16:22:14.000000 libhmac-20240417/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-17 19:07:40.000000 libhmac-20240417/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-17 19:07:40.000000 libhmac-20240417/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:18.000000 libhmac-20240417/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-17 19:07:40.000000 libhmac-20240417/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:18.000000 libhmac-20240417/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:18.000000 libhmac-20240417/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-17 19:07:41.000000 libhmac-20240417/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:18.000000 libhmac-20240417/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:18.000000 libhmac-20240417/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-17 19:07:40.000000 libhmac-20240417/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:18.000000 libhmac-20240417/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6400 2024-04-17 16:22:14.000000 libhmac-20240417/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-04-17 16:22:14.000000 libhmac-20240417/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:18.000000 libhmac-20240417/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-17 16:22:14.000000 libhmac-20240417/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      388 2024-04-17 18:53:45.000000 libhmac-20240417/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18774 2024-04-17 16:22:11.000000 libhmac-20240417/include/libhmac.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/include/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2024-04-17 16:22:11.000000 libhmac-20240417/include/libhmac/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-04-17 19:08:02.000000 libhmac-20240417/include/libhmac/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5110 2024-04-17 16:22:11.000000 libhmac-20240417/include/libhmac/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4979 2024-04-17 19:08:03.000000 libhmac-20240417/include/libhmac/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 16:23:50.000000 libhmac-20240417/include/libhmac/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-17 16:22:11.000000 libhmac-20240417/include/libhmac/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 16:22:11.000000 libhmac-20240417/include/libhmac/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 19:08:03.000000 libhmac-20240417/include/libhmac/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24856 2024-04-17 19:07:45.000000 libhmac-20240417/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18774 2024-04-17 19:08:02.000000 libhmac-20240417/include/libhmac.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-17 16:22:11.000000 libhmac-20240417/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-17 16:22:11.000000 libhmac-20240417/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-17 16:22:11.000000 libhmac-20240417/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-17 16:22:11.000000 libhmac-20240417/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-17 16:22:11.000000 libhmac-20240417/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-17 16:22:11.000000 libhmac-20240417/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-17 16:22:11.000000 libhmac-20240417/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-17 18:53:45.000000 libhmac-20240417/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-17 16:22:11.000000 libhmac-20240417/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-17 19:08:03.000000 libhmac-20240417/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14987 2024-04-17 19:07:44.000000 libhmac-20240417/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15866 2024-04-17 19:06:56.000000 libhmac-20240417/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-17 16:22:11.000000 libhmac-20240417/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-17 16:22:11.000000 libhmac-20240417/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-17 16:22:11.000000 libhmac-20240417/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21931 2024-04-17 19:07:45.000000 libhmac-20240417/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27129 2024-04-17 19:07:45.000000 libhmac-20240417/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 19:07:27.000000 libhmac-20240417/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-17 18:54:19.000000 libhmac-20240417/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:10:17.000000 libhmac-20240417/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-17 19:07:45.000000 libhmac-20240417/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/libhmac.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-17 16:22:14.000000 libhmac-20240417/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/libhmac-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2165 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-17 19:08:03.000000 libhmac-20240417/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/libhmac-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-17 16:22:09.000000 libhmac-20240417/dpkg/libhmac-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-04-17 19:08:03.000000 libhmac-20240417/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-17 16:22:09.000000 libhmac-20240417/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1455921 2024-04-17 19:07:43.000000 libhmac-20240417/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-17 19:07:45.000000 libhmac-20240417/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-17 19:07:45.000000 libhmac-20240417/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmacsum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6731 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmacsum/hmacsum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha256/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/hmac_test_sha256/hmac_test_sha256.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha1_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_sha1_context/hmac_test_sha1_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_md5_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4881 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_md5_context/hmac_test_md5_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1013 2024-04-17 18:54:30.000000 libhmac-20240417/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha1/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4860 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/hmac_test_sha1/hmac_test_sha1.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha512_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_sha512_context/hmac_test_sha512_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha512/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/hmac_test_sha512/hmac_test_sha512.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4626 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_support/hmac_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha224_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_sha224_context/hmac_test_sha224_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha256_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_sha256_context/hmac_test_sha256_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_md5/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4857 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/hmac_test_md5/hmac_test_md5.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4620 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/hmac_test_error/hmac_test_error.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17036 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/libhmac.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6796 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/hmac_test_sha224/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-04-17 16:22:55.000000 libhmac-20240417/msvscpp/hmac_test_sha224/hmac_test_sha224.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19934 2024-04-17 19:07:45.000000 libhmac-20240417/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/pyhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6513 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/pyhmac/pyhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:54.000000 libhmac-20240417/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-17 16:22:27.000000 libhmac-20240417/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      197 2024-04-17 16:22:11.000000 libhmac-20240417/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:52.000000 libhmac-20240417/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27962 2024-04-17 19:07:45.000000 libhmac-20240417/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-17 19:07:26.000000 libhmac-20240417/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      320 2024-04-17 16:22:09.000000 libhmac-20240417/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-17 19:07:45.000000 libhmac-20240417/INSTALL
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      358 2024-04-17 16:22:09.000000 libhmac-20240417/libhmac.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 16:22:09.000000 libhmac-20240417/pyproject.toml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:52.000000 libhmac-20240417/hmactools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_system_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3376 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1314 2024-04-17 18:54:41.000000 libhmac-20240417/hmactools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4142 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4799 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/sum_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8333 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmacsum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38351 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/sum_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29109 2024-04-17 19:07:45.000000 libhmac-20240417/hmactools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1267 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-04-17 16:22:13.000000 libhmac-20240417/hmactools/hmactools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-17 16:22:09.000000 libhmac-20240417/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-17 19:07:45.000000 libhmac-20240417/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-17 16:22:09.000000 libhmac-20240417/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2024-04-17 16:22:55.000000 libhmac-20240417/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:10:17.000000 libhmac-20240417/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30314 2024-04-17 19:07:45.000000 libhmac-20240417/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-17 19:07:33.000000 libhmac-20240417/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-17 19:07:45.000000 libhmac-20240417/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:52.000000 libhmac-20240417/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27160 2024-04-17 19:07:45.000000 libhmac-20240417/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-17 19:07:30.000000 libhmac-20240417/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3043 2024-04-17 16:22:09.000000 libhmac-20240417/libhmac.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 09:10:19.000000 libhmac-20240417/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2024-04-17 16:22:14.000000 libhmac-20240417/manuals/hmacsum.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-04-17 18:54:49.000000 libhmac-20240417/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-04-17 16:22:14.000000 libhmac-20240417/manuals/libhmac.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23888 2024-04-17 19:07:45.000000 libhmac-20240417/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27739 2024-04-17 16:22:55.000000 libhmac-20240417/tests/hmac_test_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7073 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_md5.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/tests/input/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/tests/input/public/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/empty
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       64 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test8
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       56 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test7
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test2
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       80 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test6
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       62 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test5
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       26 2023-12-03 09:10:16.000000 libhmac-20240417/tests/input/public/test4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15803 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14435 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14579 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28073 2024-04-17 16:22:55.000000 libhmac-20240417/tests/hmac_test_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4122 2024-04-17 18:55:01.000000 libhmac-20240417/tests/Makefile.am
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5619 2024-04-17 18:50:02.000000 libhmac-20240417/tests/test_sha2sum.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4408 2024-04-17 18:49:50.000000 libhmac-20240417/tests/test_md5sum.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 16:22:13.000000 libhmac-20240417/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4380 2024-04-17 16:22:13.000000 libhmac-20240417/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 16:22:13.000000 libhmac-20240417/tests/hmac_test_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-17 16:22:13.000000 libhmac-20240417/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28089 2024-04-17 16:22:55.000000 libhmac-20240417/tests/hmac_test_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 16:22:13.000000 libhmac-20240417/tests/hmac_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7018 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-17 16:22:14.000000 libhmac-20240417/tests/hmac_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28090 2024-04-17 16:22:55.000000 libhmac-20240417/tests/hmac_test_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52713 2024-04-17 19:07:45.000000 libhmac-20240417/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-17 16:22:13.000000 libhmac-20240417/tests/hmac_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27584 2024-04-17 16:22:55.000000 libhmac-20240417/tests/hmac_test_md5_context.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4430 2024-04-17 18:50:16.000000 libhmac-20240417/tests/test_sha1sum.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-17 16:22:13.000000 libhmac-20240417/tests/pyhmac_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4120 2024-04-17 16:25:02.000000 libhmac-20240417/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/sha512_context_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1224 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/sha1_context_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1937 2024-04-17 18:55:26.000000 libhmac-20240417/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/ossfuzz_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1218 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/md5_context_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/sha256_context_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34729 2024-04-17 19:07:45.000000 libhmac-20240417/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1237 2024-04-17 16:22:12.000000 libhmac-20240417/ossfuzz/sha224_context_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-17 19:07:40.000000 libhmac-20240417/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-04-17 19:08:03.000000 libhmac-20240417/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1393 2024-04-17 18:55:42.000000 libhmac-20240417/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1100 2024-04-17 19:08:03.000000 libhmac-20240417/libhmac/libhmac.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31831 2024-04-17 19:07:45.000000 libhmac-20240417/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-04-17 16:22:12.000000 libhmac-20240417/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28057 2024-04-17 19:07:45.000000 libhmac-20240417/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-17 19:07:31.000000 libhmac-20240417/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:18.000000 libhmac-20240417/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:18.000000 libhmac-20240417/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:18.000000 libhmac-20240417/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:18.000000 libhmac-20240417/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:18.000000 libhmac-20240417/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:18.000000 libhmac-20240417/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:18.000000 libhmac-20240417/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:18.000000 libhmac-20240417/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:18.000000 libhmac-20240417/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-17 19:08:02.000000 libhmac-20240417/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:18.000000 libhmac-20240417/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:18.000000 libhmac-20240417/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:52.000000 libhmac-20240417/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53641 2024-04-17 19:07:45.000000 libhmac-20240417/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-17 19:07:35.000000 libhmac-20240417/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37129 2024-04-17 19:07:45.000000 libhmac-20240417/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:53.000000 libhmac-20240417/pyhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1953 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7203 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9771 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1343 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 18:55:10.000000 libhmac-20240417/pyhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1337 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7233 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7909 2024-04-17 16:22:55.000000 libhmac-20240417/pyhmac/pyhmac.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-04-17 16:22:13.000000 libhmac-20240417/pyhmac/pyhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9967 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46362 2024-04-17 19:07:45.000000 libhmac-20240417/pyhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9673 2024-04-17 16:22:12.000000 libhmac-20240417/pyhmac/pyhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26998 2024-04-17 19:07:45.000000 libhmac-20240417/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-17 19:07:29.000000 libhmac-20240417/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-18 01:43:51.000000 libhmac-20240417/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-17 19:07:24.000000 libhmac-20240417/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26465 2024-04-17 19:07:45.000000 libhmac-20240417/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56650 2024-04-17 19:07:42.000000 libhmac-20240417/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6264 2024-04-17 16:22:09.000000 libhmac-20240417/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-04-18 01:43:54.829335 libhmac-20240417/PKG-INFO
```

### Comparing `libhmac-20240129/COPYING` & `libhmac-20240417/COPYING`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/install-sh` & `libhmac-20240417/install-sh`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac.spec` & `libhmac-20240417/libhmac.spec`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libhmac
-Version: 20240129
+Version: 20240417
 Release: 1
 Summary: Library to support various Hash-based Message Authentication Codes (HMAC)
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libhmac
 Requires:  openssl 
@@ -91,10 +91,10 @@
 %files -n libhmac-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Mon Jan 29 2024 Joachim Metz <joachim.metz@gmail.com> 20240129-1
+* Wed Apr 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240417-1
 - Auto-generated
```

### Comparing `libhmac-20240129/depcomp` & `libhmac-20240417/depcomp`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libcfile.m4` & `libhmac-20240417/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/tests.m4` & `libhmac-20240417/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libcpath.m4` & `libhmac-20240417/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/lib-prefix.m4` & `libhmac-20240417/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/progtest.m4` & `libhmac-20240417/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libuna.m4` & `libhmac-20240417/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/gettext.m4` & `libhmac-20240417/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/lib-ld.m4` & `libhmac-20240417/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libclocale.m4` & `libhmac-20240417/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/libcsplit.m4` & `libhmac-20240417/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/common.m4` & `libhmac-20240417/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libhmac-20240129/m4/libcthreads.m4` & `libhmac-20240417/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libhmac-20240129/m4/ltversion.m4` & `libhmac-20240417/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/ltsugar.m4` & `libhmac-20240417/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/host-cpu-c-abi.m4` & `libhmac-20240417/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libtool.m4` & `libhmac-20240417/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/po.m4` & `libhmac-20240417/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/libcerror.m4` & `libhmac-20240417/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/libcnotify.m4` & `libhmac-20240417/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libhmac-20240129/m4/intlmacosx.m4` & `libhmac-20240417/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/lt~obsolete.m4` & `libhmac-20240417/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/lib-link.m4` & `libhmac-20240417/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/iconv.m4` & `libhmac-20240417/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/ltoptions.m4` & `libhmac-20240417/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/nls.m4` & `libhmac-20240417/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/python.m4` & `libhmac-20240417/m4/python.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240416
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,19 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
       [$host_os],
       [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libhmac-20240129/m4/libcrypto.m4` & `libhmac-20240417/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libhmac-20240129/m4/types.m4` & `libhmac-20240417/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/m4/pthread.m4` & `libhmac-20240417/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libhmac-20240129/include/libhmac.h.in` & `libhmac-20240417/include/libhmac.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/definitions.h.in` & `libhmac-20240417/include/libhmac/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/definitions.h` & `libhmac-20240417/include/libhmac/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBHMAC_DEFINITIONS_H )
 #define _LIBHMAC_DEFINITIONS_H
 
 #include <libhmac/types.h>
 
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libhmac-20240129/include/libhmac/types.h.in` & `libhmac-20240417/include/libhmac/types.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/types.h` & `libhmac-20240417/include/libhmac/types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/features.h.in` & `libhmac-20240417/include/libhmac/features.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/error.h` & `libhmac-20240417/include/libhmac/error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/extern.h` & `libhmac-20240417/include/libhmac/extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/libhmac/features.h` & `libhmac-20240417/include/libhmac/features.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/include/Makefile.in` & `libhmac-20240417/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,20 @@
 
 EXTRA_DIST = \
 	libhmac.h.in \
 	libhmac/definitions.h.in \
 	libhmac/features.h.in \
 	libhmac/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libhmac.h \
+	libhmac/definitions.h \
+	libhmac/features.h \
+	libhmac/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -664,23 +669,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -762,17 +769,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libhmac.h
-	-rm -f libhmac/definitions.h
-	-rm -f libhmac/features.h
-	-rm -f libhmac/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/include/libhmac.h` & `libhmac-20240417/include/libhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/config_borlandc.h` & `libhmac-20240417/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/file_stream.h` & `libhmac-20240417/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/memory.h` & `libhmac-20240417/common/memory.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/byte_stream.h` & `libhmac-20240417/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/common.h` & `libhmac-20240417/common/common.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/config_winapi.h` & `libhmac-20240417/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/system_string.h` & `libhmac-20240417/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/types.h.in` & `libhmac-20240417/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/types.h` & `libhmac-20240417/common/types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/config.h.in` & `libhmac-20240417/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/config.h` & `libhmac-20240417/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -490,24 +490,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libhmac"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libhmac 20240129"
+#define PACKAGE_STRING "libhmac 20240417"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libhmac"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240129"
+#define PACKAGE_VERSION "20240417"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -525,15 +525,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240129"
+#define VERSION "20240417"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libhmac-20240129/common/wide_string.h` & `libhmac-20240417/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/narrow_string.h` & `libhmac-20240417/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/config_msc.h` & `libhmac-20240417/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/common/Makefile.in` & `libhmac-20240417/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -429,15 +431,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -605,23 +610,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -701,15 +708,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/libclocale/libclocale_wide_string.c` & `libhmac-20240417/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_support.h` & `libhmac-20240417/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/Makefile.am` & `libhmac-20240417/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libhmac-20240129/libclocale/libclocale_definitions.h` & `libhmac-20240417/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libhmac-20240129/libclocale/libclocale_unused.h` & `libhmac-20240417/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_libcerror.h` & `libhmac-20240417/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_locale.h` & `libhmac-20240417/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_support.c` & `libhmac-20240417/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_codepage.c` & `libhmac-20240417/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_locale.c` & `libhmac-20240417/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/Makefile.in` & `libhmac-20240417/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -459,30 +459,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -685,24 +686,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -789,17 +796,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libclocale/libclocale_extern.h` & `libhmac-20240417/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_wide_string.h` & `libhmac-20240417/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libclocale/libclocale_codepage.h` & `libhmac-20240417/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/config.guess` & `libhmac-20240417/config.guess`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/dpkg/copyright` & `libhmac-20240417/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/dpkg/control` & `libhmac-20240417/dpkg/control`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/dpkg/rules` & `libhmac-20240417/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/COPYING.LESSER` & `libhmac-20240417/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/configure` & `libhmac-20240417/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libhmac 20240129.
+# Generated by GNU Autoconf 2.71 for libhmac 20240417.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libhmac'
 PACKAGE_TARNAME='libhmac'
-PACKAGE_VERSION='20240129'
-PACKAGE_STRING='libhmac 20240129'
+PACKAGE_VERSION='20240417'
+PACKAGE_STRING='libhmac 20240417'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libhmac.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1568,15 +1568,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libhmac 20240129 to adapt to many kinds of systems.
+\`configure' configures libhmac 20240417 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1639,15 +1639,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libhmac 20240129:";;
+     short | recursive ) echo "Configuration of libhmac 20240417:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1851,15 +1851,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libhmac configure 20240129
+libhmac configure 20240417
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2572,15 +2572,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libhmac $as_me 20240129, which was
+It was created by libhmac $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4061,15 +4061,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libhmac'
- VERSION='20240129'
+ VERSION='20240417'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23594,15 +23594,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24093,15 +24093,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24243,15 +24244,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24345,15 +24346,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -25985,15 +25986,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26047,47 +26048,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26121,15 +26127,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26163,15 +26169,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26206,15 +26212,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26248,15 +26254,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26290,15 +26296,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26332,15 +26338,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26374,15 +26380,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26417,15 +26423,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26459,15 +26465,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26501,15 +26507,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26543,15 +26549,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26585,15 +26591,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26628,15 +26634,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26670,15 +26676,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26712,15 +26718,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26754,15 +26760,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26796,15 +26802,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26839,67 +26845,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27028,15 +27043,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -27392,15 +27407,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31840,14 +31855,16 @@
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
         case $host_os in #(
   cygwin*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
         BACKUP_CPPFLAGS="${CPPFLAGS}"
@@ -32009,15 +32026,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32564,15 +32581,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32728,15 +32746,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -32806,15 +32824,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33264,15 +33282,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33327,15 +33346,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -33405,15 +33424,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -34128,15 +34147,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -34161,15 +34181,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -34239,15 +34259,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41449,15 +41469,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -41482,15 +41503,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -41560,15 +41581,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42749,15 +42770,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43071,15 +43093,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -43149,15 +43171,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43954,15 +43976,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -44152,15 +44175,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -45049,15 +45072,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libhmac $as_me 20240129, which was
+This file was extended by libhmac $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -45117,15 +45140,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libhmac config.status 20240129
+libhmac config.status 20240417
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libhmac-20240129/compile` & `libhmac-20240417/compile`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/missing` & `libhmac-20240417/missing`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmacsum/hmacsum.vcproj` & `libhmac-20240417/msvscpp/hmacsum/hmacsum.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha256/hmac_test_sha256.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha256/hmac_test_sha256.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha1_context/hmac_test_sha1_context.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha1_context/hmac_test_sha1_context.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_md5_context/hmac_test_md5_context.vcproj` & `libhmac-20240417/msvscpp/hmac_test_md5_context/hmac_test_md5_context.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libclocale/libclocale.vcproj` & `libhmac-20240417/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/Makefile.am` & `libhmac-20240417/msvscpp/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -23,13 +23,11 @@
 	libuna/libuna.vcproj \
 	pyhmac/pyhmac.vcproj \
 	libhmac.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha1/hmac_test_sha1.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha1/hmac_test_sha1.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha512_context/hmac_test_sha512_context.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha512_context/hmac_test_sha512_context.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha512/hmac_test_sha512.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha512/hmac_test_sha512.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcfile/libcfile.vcproj` & `libhmac-20240417/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_support/hmac_test_support.vcproj` & `libhmac-20240417/msvscpp/hmac_test_support/hmac_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha224_context/hmac_test_sha224_context.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha224_context/hmac_test_sha224_context.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha256_context/hmac_test_sha256_context.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha256_context/hmac_test_sha256_context.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_md5/hmac_test_md5.vcproj` & `libhmac-20240417/msvscpp/hmac_test_md5/hmac_test_md5.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_error/hmac_test_error.vcproj` & `libhmac-20240417/msvscpp/hmac_test_error/hmac_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libhmac.sln` & `libhmac-20240417/msvscpp/libhmac.sln`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcthreads/libcthreads.vcproj` & `libhmac-20240417/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcpath/libcpath.vcproj` & `libhmac-20240417/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libhmac/libhmac.vcproj` & `libhmac-20240417/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/hmac_test_sha224/hmac_test_sha224.vcproj` & `libhmac-20240417/msvscpp/hmac_test_sha224/hmac_test_sha224.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcsplit/libcsplit.vcproj` & `libhmac-20240417/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libuna/libuna.vcproj` & `libhmac-20240417/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/Makefile.in` & `libhmac-20240417/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -424,15 +424,16 @@
 	libuna/libuna.vcproj \
 	pyhmac/pyhmac.vcproj \
 	libhmac.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -536,23 +537,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -631,13 +634,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/msvscpp/pyhmac/pyhmac.vcproj` & `libhmac-20240417/msvscpp/pyhmac/pyhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcnotify/libcnotify.vcproj` & `libhmac-20240417/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/msvscpp/libcerror/libcerror.vcproj` & `libhmac-20240417/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_extern.h` & `libhmac-20240417/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_support.h` & `libhmac-20240417/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_unused.h` & `libhmac-20240417/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_notify.h` & `libhmac-20240417/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_support.c` & `libhmac-20240417/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_types.h` & `libhmac-20240417/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/Makefile.am` & `libhmac-20240417/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libhmac-20240129/libcfile/libcfile_notify.c` & `libhmac-20240417/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_system_string.h` & `libhmac-20240417/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_file.h` & `libhmac-20240417/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_libcnotify.h` & `libhmac-20240417/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_system_string.c` & `libhmac-20240417/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_error.h` & `libhmac-20240417/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_libcerror.h` & `libhmac-20240417/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_file.c` & `libhmac-20240417/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_libclocale.h` & `libhmac-20240417/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_winapi.h` & `libhmac-20240417/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/Makefile.in` & `libhmac-20240417/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -461,16 +461,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -485,15 +485,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -698,24 +699,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -804,17 +813,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libcfile/libcfile_error.c` & `libhmac-20240417/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_libuna.h` & `libhmac-20240417/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_winapi.c` & `libhmac-20240417/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcfile/libcfile_definitions.h` & `libhmac-20240417/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libhmac-20240129/INSTALL` & `libhmac-20240417/INSTALL`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libcpath.h` & `libhmac-20240417/hmactools/hmactools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_output.h` & `libhmac-20240417/hmactools/hmactools_output.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_system_split_string.h` & `libhmac-20240417/hmactools/hmactools_system_split_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_signal.c` & `libhmac-20240417/hmactools/hmactools_signal.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/digest_hash.c` & `libhmac-20240417/hmactools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/byte_size_string.c` & `libhmac-20240417/hmactools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/Makefile.am` & `libhmac-20240417/hmactools/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -44,17 +44,15 @@
 	../libhmac/libhmac.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on hmacsum ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(hmacsum_SOURCES)
```

### Comparing `libhmac-20240129/hmactools/hmactools_signal.h` & `libhmac-20240417/hmactools/hmactools_signal.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_output.c` & `libhmac-20240417/hmactools/hmactools_output.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libuna.h` & `libhmac-20240417/hmactools/hmactools_libuna.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libcnotify.h` & `libhmac-20240417/hmactools/hmactools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libcfile.h` & `libhmac-20240417/hmactools/hmactools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_i18n.h` & `libhmac-20240417/hmactools/hmactools_i18n.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libcerror.h` & `libhmac-20240417/hmactools/hmactools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/sum_handle.h` & `libhmac-20240417/hmactools/sum_handle.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmacsum.c` & `libhmac-20240417/hmactools/hmacsum.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libhmac.h` & `libhmac-20240417/hmactools/hmactools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_getopt.h` & `libhmac-20240417/hmactools/hmactools_getopt.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_unused.h` & `libhmac-20240417/hmactools/hmactools_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libcsplit.h` & `libhmac-20240417/hmactools/hmactools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/sum_handle.c` & `libhmac-20240417/hmactools/sum_handle.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/Makefile.in` & `libhmac-20240417/hmactools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -453,16 +453,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -498,15 +498,16 @@
 	../libhmac/libhmac.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -754,23 +755,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/digest_hash.Po
+	-rm -f ./$(DEPDIR)/hmacsum.Po
+	-rm -f ./$(DEPDIR)/hmactools_getopt.Po
+	-rm -f ./$(DEPDIR)/hmactools_output.Po
+	-rm -f ./$(DEPDIR)/hmactools_signal.Po
+	-rm -f ./$(DEPDIR)/sum_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,17 +870,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on hmacsum ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(hmacsum_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/hmactools/byte_size_string.h` & `libhmac-20240417/hmactools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/digest_hash.h` & `libhmac-20240417/hmactools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_getopt.c` & `libhmac-20240417/hmactools/hmactools_getopt.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/hmactools/hmactools_libclocale.h` & `libhmac-20240417/hmactools/hmactools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/config.sub` & `libhmac-20240417/config.sub`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/setup.py` & `libhmac-20240417/setup.py`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/acinclude.m4` & `libhmac-20240417/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/config.rpath` & `libhmac-20240417/config.rpath`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread.h` & `libhmac-20240417/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_read_write_lock.h` & `libhmac-20240417/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread.c` & `libhmac-20240417/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread_pool.h` & `libhmac-20240417/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_support.h` & `libhmac-20240417/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_lock.h` & `libhmac-20240417/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_unused.h` & `libhmac-20240417/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_lock.c` & `libhmac-20240417/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_condition.h` & `libhmac-20240417/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_repeating_thread.h` & `libhmac-20240417/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/Makefile.am` & `libhmac-20240417/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libhmac-20240129/libcthreads/libcthreads_support.c` & `libhmac-20240417/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_mutex.c` & `libhmac-20240417/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_queue.c` & `libhmac-20240417/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_mutex.h` & `libhmac-20240417/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_types.h` & `libhmac-20240417/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread_attributes.h` & `libhmac-20240417/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_condition.c` & `libhmac-20240417/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_error.c` & `libhmac-20240417/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_read_write_lock.c` & `libhmac-20240417/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_libcerror.h` & `libhmac-20240417/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_definitions.h` & `libhmac-20240417/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread_pool.c` & `libhmac-20240417/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_error.h` & `libhmac-20240417/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_thread_attributes.c` & `libhmac-20240417/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_extern.h` & `libhmac-20240417/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/libcthreads_repeating_thread.c` & `libhmac-20240417/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcthreads/Makefile.in` & `libhmac-20240417/libcthreads/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -479,16 +479,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -503,15 +503,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -721,24 +722,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -832,17 +846,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libcthreads/libcthreads_queue.h` & `libhmac-20240417/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/test-driver` & `libhmac-20240417/test-driver`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_support.c` & `libhmac-20240417/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_libcerror.h` & `libhmac-20240417/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_definitions.h` & `libhmac-20240417/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libhmac-20240129/libcpath/Makefile.am` & `libhmac-20240417/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libhmac-20240129/libcpath/libcpath_error.c` & `libhmac-20240417/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_extern.h` & `libhmac-20240417/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_system_string.h` & `libhmac-20240417/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_support.h` & `libhmac-20240417/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_libcsplit.h` & `libhmac-20240417/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_system_string.c` & `libhmac-20240417/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_libclocale.h` & `libhmac-20240417/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_error.h` & `libhmac-20240417/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/Makefile.in` & `libhmac-20240417/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -455,16 +455,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -476,15 +476,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -687,24 +688,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -791,17 +798,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libcpath/libcpath_libuna.h` & `libhmac-20240417/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_unused.h` & `libhmac-20240417/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_path.c` & `libhmac-20240417/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcpath/libcpath_path.h` & `libhmac-20240417/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac.spec.in` & `libhmac-20240417/libhmac.spec.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ChangeLog` & `libhmac-20240417/ChangeLog`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/manuals/hmacsum.1` & `libhmac-20240417/manuals/hmacsum.1`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/manuals/libhmac.3` & `libhmac-20240417/manuals/libhmac.3`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/manuals/Makefile.in` & `libhmac-20240417/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,16 @@
 	hmacsum.1 \
 	libhmac.3
 
 EXTRA_DIST = \
 	hmacsum.1 \
 	libhmac.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -636,23 +637,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -734,13 +737,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/tests/hmac_test_sha1_context.c` & `libhmac-20240417/tests/hmac_test_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_md5.c` & `libhmac-20240417/tests/hmac_test_md5.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha512.c` & `libhmac-20240417/tests/hmac_test_sha512.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha224.c` & `libhmac-20240417/tests/hmac_test_sha224.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha256.c` & `libhmac-20240417/tests/hmac_test_sha256.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha256_context.c` & `libhmac-20240417/tests/hmac_test_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_memory.c` & `libhmac-20240417/tests/hmac_test_memory.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/Makefile.am` & `libhmac-20240417/tests/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBHMAC_DLL_IMPORT@
 
 if HAVE_PYTHON_TESTS
 TESTS_PYHMAC = \
@@ -191,13 +191,11 @@
 hmac_test_support_LDADD = \
 	../libhmac/libhmac.la
 
 EXTRA_DIST = \
 	$(check_SCRIPTS) \
 	$(TESTS_INPUT)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libhmac-20240129/tests/test_sha2sum.sh` & `libhmac-20240417/tests/test_sha2sum.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Sum tool testing script
 #
-# Version: 20231007
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("hmacsum");
 OPTIONS_PER_PROFILE=("")
@@ -105,20 +105,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libhmac-20240129/tests/test_md5sum.sh` & `libhmac-20240417/tests/test_md5sum.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Sum tool testing script
 #
-# Version: 20231007
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("hmacsum");
 OPTIONS_PER_PROFILE=("")
@@ -71,20 +71,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libhmac-20240129/tests/test_python_module.sh` & `libhmac-20240417/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240416
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libhmac";
+PYTHON_MODULE="pyhmac";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyhmac_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyhmac_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyhmac");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/${LIBRARY_NAME}-1.dll ../${PYTHON_MODULE}/libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libhmac-20240129/tests/hmac_test_libhmac.h` & `libhmac-20240417/tests/hmac_test_libhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_memory.h` & `libhmac-20240417/tests/hmac_test_memory.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/test_runner.sh` & `libhmac-20240417/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha224_context.c` & `libhmac-20240417/tests/hmac_test_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_unused.h` & `libhmac-20240417/tests/hmac_test_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_support.c` & `libhmac-20240417/tests/hmac_test_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_libcerror.h` & `libhmac-20240417/tests/hmac_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha1.c` & `libhmac-20240417/tests/hmac_test_sha1.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_macros.h` & `libhmac-20240417/tests/hmac_test_macros.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_sha512_context.c` & `libhmac-20240417/tests/hmac_test_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/Makefile.in` & `libhmac-20240417/tests/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -727,16 +727,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBHMAC_DLL_IMPORT@
 
 @HAVE_PYTHON_TESTS_TRUE@TESTS_PYHMAC = \
 @HAVE_PYTHON_TESTS_TRUE@	test_python_module.sh
@@ -907,15 +907,16 @@
 hmac_test_support_LDADD = \
 	../libhmac/libhmac.la
 
 EXTRA_DIST = \
 	$(check_SCRIPTS) \
 	$(TESTS_INPUT)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1366,24 +1367,39 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/hmac_test_error.Po
+	-rm -f ./$(DEPDIR)/hmac_test_md5.Po
+	-rm -f ./$(DEPDIR)/hmac_test_md5_context.Po
+	-rm -f ./$(DEPDIR)/hmac_test_memory.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha1.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha1_context.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha224.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha224_context.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha256.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha256_context.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha512.Po
+	-rm -f ./$(DEPDIR)/hmac_test_sha512_context.Po
+	-rm -f ./$(DEPDIR)/hmac_test_support.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1479,13 +1495,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/tests/hmac_test_error.c` & `libhmac-20240417/tests/hmac_test_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/hmac_test_md5_context.c` & `libhmac-20240417/tests/hmac_test_md5_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/test_sha1sum.sh` & `libhmac-20240417/tests/test_sha1sum.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Sum tool testing script
 #
-# Version: 20231007
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("hmacsum");
 OPTIONS_PER_PROFILE=("")
@@ -73,20 +73,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libhmac-20240129/tests/pyhmac_test_support.py` & `libhmac-20240417/tests/pyhmac_test_support.py`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/tests/test_library.sh` & `libhmac-20240417/tests/test_library.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="error md5 md5_context sha1 sha1_context sha224 sha224_context sha256 sha256_context sha512 sha512_context support";
 LIBRARY_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libhmac-20240129/ossfuzz/sha512_context_fuzzer.cc` & `libhmac-20240417/ossfuzz/sha512_context_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ossfuzz/sha1_context_fuzzer.cc` & `libhmac-20240417/ossfuzz/sha1_context_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ossfuzz/Makefile.am` & `libhmac-20240417/ossfuzz/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	md5_context_fuzzer \
 	sha1_context_fuzzer \
 	sha224_context_fuzzer \
 	sha256_context_fuzzer \
 	sha512_context_fuzzer
@@ -47,20 +47,18 @@
 	ossfuzz_libhmac.h
 
 sha512_context_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libhmac/libhmac.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on md5_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(md5_context_fuzzer_SOURCES)
 	@echo "Running splint on sha1_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sha1_context_fuzzer_SOURCES)
 	@echo "Running splint on sha224_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sha224_context_fuzzer_SOURCES)
```

### Comparing `libhmac-20240129/ossfuzz/ossfuzz_libhmac.h` & `libhmac-20240417/ossfuzz/ossfuzz_libhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ossfuzz/md5_context_fuzzer.cc` & `libhmac-20240417/ossfuzz/md5_context_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ossfuzz/sha256_context_fuzzer.cc` & `libhmac-20240417/ossfuzz/sha256_context_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ossfuzz/Makefile.in` & `libhmac-20240417/ossfuzz/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -512,16 +512,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@md5_context_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	md5_context_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libhmac.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@md5_context_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -555,15 +555,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	sha512_context_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libhmac.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@sha512_context_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libhmac/libhmac.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -825,23 +826,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/md5_context_fuzzer.Po
+	-rm -f ./$(DEPDIR)/sha1_context_fuzzer.Po
+	-rm -f ./$(DEPDIR)/sha224_context_fuzzer.Po
+	-rm -f ./$(DEPDIR)/sha256_context_fuzzer.Po
+	-rm -f ./$(DEPDIR)/sha512_context_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -929,17 +937,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on md5_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(md5_context_fuzzer_SOURCES)
 	@echo "Running splint on sha1_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sha1_context_fuzzer_SOURCES)
 	@echo "Running splint on sha224_context_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sha224_context_fuzzer_SOURCES)
```

### Comparing `libhmac-20240129/ossfuzz/sha224_context_fuzzer.cc` & `libhmac-20240417/ossfuzz/sha224_context_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/ltmain.sh` & `libhmac-20240417/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha1_context.c` & `libhmac-20240417/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha224.h` & `libhmac-20240417/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha512_context.c` & `libhmac-20240417/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_extern.h` & `libhmac-20240417/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_md5.c` & `libhmac-20240417/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_md5.h` & `libhmac-20240417/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_error.h` & `libhmac-20240417/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_types.h` & `libhmac-20240417/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_byte_stream.h` & `libhmac-20240417/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha512.c` & `libhmac-20240417/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha256_context.c` & `libhmac-20240417/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha224.c` & `libhmac-20240417/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_definitions.h.in` & `libhmac-20240417/libhmac/libhmac_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_definitions.h` & `libhmac-20240417/libhmac/libhmac_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libhmac-20240129/libhmac/libhmac_unused.h` & `libhmac-20240417/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha1.h` & `libhmac-20240417/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha256_context.h` & `libhmac-20240417/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/Makefile.am` & `libhmac-20240417/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBHMAC_DLL_EXPORT@
 
 lib_LTLIBRARIES = libhmac.la
 
@@ -38,21 +38,19 @@
 libhmac_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libhmac_definitions.h.in \
 	libhmac.rc \
 	libhmac.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libhmac_definitions.h \
+	libhmac.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libhmac_definitions.h
-	-rm -f libhmac.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libhmac-20240129/libhmac/libhmac.rc` & `libhmac-20240417/libhmac/libhmac.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support various Hash-based Message Authentication Codes (HMAC)\0"
-      VALUE "FileVersion",		"20240129" "\0"
+      VALUE "FileVersion",		"20240417" "\0"
       VALUE "InternalName",		"libhmac.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libhmac.dll\0"
       VALUE "ProductName",		"libhmac\0"
-      VALUE "ProductVersion",		"20240129" "\0"
+      VALUE "ProductVersion",		"20240417" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libhmac/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libhmac-20240129/libhmac/libhmac_sha224_context.c` & `libhmac-20240417/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_md5_context.h` & `libhmac-20240417/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha256.c` & `libhmac-20240417/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac.rc.in` & `libhmac-20240417/libhmac/libhmac.rc.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha1_context.h` & `libhmac-20240417/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_libcerror.h` & `libhmac-20240417/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_error.c` & `libhmac-20240417/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_support.h` & `libhmac-20240417/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac.c` & `libhmac-20240417/libhmac/libhmac.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/Makefile.in` & `libhmac-20240417/libhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -491,16 +491,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBHMAC_DLL_EXPORT@
 
 lib_LTLIBRARIES = libhmac.la
 libhmac_la_SOURCES = \
@@ -532,15 +532,18 @@
 
 libhmac_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libhmac_definitions.h.in \
 	libhmac.rc \
 	libhmac.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libhmac_definitions.h \
+	libhmac.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -783,24 +786,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac.Plo
+	-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -896,19 +914,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libhmac_definitions.h
-	-rm -f libhmac.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libhmac/libhmac_sha256.h` & `libhmac-20240417/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha224_context.h` & `libhmac-20240417/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha512_context.h` & `libhmac-20240417/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha512.h` & `libhmac-20240417/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_support.c` & `libhmac-20240417/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_sha1.c` & `libhmac-20240417/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libhmac/libhmac_md5_context.c` & `libhmac-20240417/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_narrow_string.c` & `libhmac-20240417/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_definitions.h` & `libhmac-20240417/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libhmac-20240129/libcsplit/libcsplit_types.h` & `libhmac-20240417/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_wide_split_string.c` & `libhmac-20240417/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_support.h` & `libhmac-20240417/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/Makefile.am` & `libhmac-20240417/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libhmac-20240129/libcsplit/libcsplit_libcerror.h` & `libhmac-20240417/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_wide_string.c` & `libhmac-20240417/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_unused.h` & `libhmac-20240417/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_wide_split_string.h` & `libhmac-20240417/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_error.c` & `libhmac-20240417/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_narrow_split_string.c` & `libhmac-20240417/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_extern.h` & `libhmac-20240417/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_error.h` & `libhmac-20240417/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_support.c` & `libhmac-20240417/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_wide_string.h` & `libhmac-20240417/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/Makefile.in` & `libhmac-20240417/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -465,16 +465,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -483,15 +483,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -696,24 +697,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -802,17 +811,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libcsplit/libcsplit_narrow_split_string.h` & `libhmac-20240417/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcsplit/libcsplit_narrow_string.h` & `libhmac-20240417/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/remove-potcdate.sin` & `libhmac-20240417/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/Makefile.in.in` & `libhmac-20240417/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/en@quot.header` & `libhmac-20240417/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/en@boldquot.header` & `libhmac-20240417/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/insert-header.sin` & `libhmac-20240417/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/Makevars` & `libhmac-20240417/po/Makevars`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/Makevars.in` & `libhmac-20240417/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/po/Rules-quot` & `libhmac-20240417/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1251.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1251.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf16_string.c` & `libhmac-20240417/libuna/libuna_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base16_stream.c` & `libhmac-20240417/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf8_stream.h` & `libhmac-20240417/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_2.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_932.c` & `libhmac-20240417/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_dingbats.h` & `libhmac-20240417/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf8_string.c` & `libhmac-20240417/libuna/libuna_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base64_stream.c` & `libhmac-20240417/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_error.h` & `libhmac-20240417/libuna/libuna_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_turkish.h` & `libhmac-20240417/libuna/libuna_codepage_mac_turkish.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_unicode_character.c` & `libhmac-20240417/libuna/libuna_unicode_character.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_gaelic.c` & `libhmac-20240417/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_arabic.h` & `libhmac-20240417/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_thai.c` & `libhmac-20240417/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_874.h` & `libhmac-20240417/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_15.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-15 codepage (Latin 9) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_15_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_utf8_string.h` & `libhmac-20240417/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_16.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1255.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf7_stream.c` & `libhmac-20240417/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_byte_stream.h` & `libhmac-20240417/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_koi8_u.c` & `libhmac-20240417/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_unused.h` & `libhmac-20240417/libuna/libuna_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_6.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_14.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base64_stream.h` & `libhmac-20240417/libuna/libuna_base64_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_error.c` & `libhmac-20240417/libuna/libuna_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_centraleurroman.h` & `libhmac-20240417/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_romanian.c` & `libhmac-20240417/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_6.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_9.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_russian.h` & `libhmac-20240417/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_dingbats.c` & `libhmac-20240417/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_15.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_936.c` & `libhmac-20240417/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_croatian.h` & `libhmac-20240417/libuna/libuna_codepage_mac_croatian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_scsu.h` & `libhmac-20240417/libuna/libuna_scsu.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/Makefile.am` & `libhmac-20240417/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,17 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libhmac-20240129/libuna/libuna_utf32_stream.c` & `libhmac-20240417/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_936.h` & `libhmac-20240417/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_10.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_roman.c` & `libhmac-20240417/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf7_stream.h` & `libhmac-20240417/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_3.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_thai.h` & `libhmac-20240417/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_farsi.h` & `libhmac-20240417/libuna/libuna_codepage_mac_farsi.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_ukrainian.c` & `libhmac-20240417/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_inuit.c` & `libhmac-20240417/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_932.h` & `libhmac-20240417/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_874.c` & `libhmac-20240417/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_5.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_10.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_definitions.h` & `libhmac-20240417/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20230710
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20230710"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libhmac-20240129/libuna/libuna_url_stream.h` & `libhmac-20240417/libuna/libuna_url_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_icelandic.h` & `libhmac-20240417/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_koi8_u.h` & `libhmac-20240417/libuna/libuna_codepage_koi8_u.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf16_stream.c` & `libhmac-20240417/libuna/libuna_utf16_stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1253.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_4.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_greek.c` & `libhmac-20240417/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_libcerror.h` & `libhmac-20240417/libuna/libuna_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_centraleurroman.c` & `libhmac-20240417/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1254.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_13.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_7.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1255.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1251.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1255 codepage (Hebrew) functions
+ * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1255_copy_from_byte_stream(
+int libuna_codepage_windows_1251_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1255_copy_to_byte_stream(
+int libuna_codepage_windows_1251_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_unicode_character.h` & `libhmac-20240417/libuna/libuna_unicode_character.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_8.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_13.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_949.h` & `libhmac-20240417/libuna/libuna_codepage_windows_949.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_cyrillic.c` & `libhmac-20240417/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_celtic.c` & `libhmac-20240417/libuna/libuna_codepage_mac_celtic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_support.h` & `libhmac-20240417/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_4.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_949.c` & `libhmac-20240417/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf16_stream.h` & `libhmac-20240417/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_symbol.c` & `libhmac-20240417/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_roman.h` & `libhmac-20240417/libuna/libuna_codepage_mac_roman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1257.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1254.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1254.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_950.c` & `libhmac-20240417/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_extern.h` & `libhmac-20240417/libuna/libuna_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1256.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_types.h` & `libhmac-20240417/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base32_stream.h` & `libhmac-20240417/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1253.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_16.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf8_stream.c` & `libhmac-20240417/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1250.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1250.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_2.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_support.c` & `libhmac-20240417/libuna/libuna_support.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_koi8_r.c` & `libhmac-20240417/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_5.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_15_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_utf16_string.h` & `libhmac-20240417/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf32_string.c` & `libhmac-20240417/libuna/libuna_utf32_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_icelandic.c` & `libhmac-20240417/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1256.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_utf32_string.h` & `libhmac-20240417/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_romanian.h` & `libhmac-20240417/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
+#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_8.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_koi8_r.h` & `libhmac-20240417/libuna/libuna_codepage_koi8_r.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_cyrillic.h` & `libhmac-20240417/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCyrillic codepage functions
+ * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
-#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
+#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
+int libuna_codepage_mac_gaelic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
+int libuna_codepage_mac_gaelic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_arabic.c` & `libhmac-20240417/libuna/libuna_codepage_mac_arabic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_croatian.c` & `libhmac-20240417/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_9.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_greek.h` & `libhmac-20240417/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1258.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1258.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_7.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/Makefile.in` & `libhmac-20240417/libuna/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -633,16 +633,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -708,15 +708,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -978,24 +979,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1115,14 +1181,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -1133,23 +1201,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_3.c` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1250.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_scsu.c` & `libhmac-20240417/libuna/libuna_scsu.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1252.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1252.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_turkish.c` & `libhmac-20240417/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_ukrainian.h` & `libhmac-20240417/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_russian.c` & `libhmac-20240417/libuna/libuna_codepage_mac_russian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1258.c` & `libhmac-20240417/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_celtic.h` & `libhmac-20240417/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_byte_stream.c` & `libhmac-20240417/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_gaelic.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1257.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacGaelic codepage functions
+ * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
-#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_gaelic_copy_from_byte_stream(
+int libuna_codepage_windows_1257_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_gaelic_copy_to_byte_stream(
+int libuna_codepage_windows_1257_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_utf32_stream.h` & `libhmac-20240417/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_symbol.h` & `libhmac-20240417/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1257.h` & `libhmac-20240417/libuna/libuna_codepage_mac_inuit.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1257 codepage (Baltic) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1257_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1257_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_inuit.h` & `libhmac-20240417/libuna/libuna_codepage_mac_romanian.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacInuit codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_mac_farsi.c` & `libhmac-20240417/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_950.h` & `libhmac-20240417/libuna/libuna_codepage_windows_950.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_url_stream.c` & `libhmac-20240417/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1251.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1255.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1251 codepage (Cyrillic) functions
+ * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1251_copy_from_byte_stream(
+int libuna_codepage_windows_1255_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1251_copy_to_byte_stream(
+int libuna_codepage_windows_1255_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_windows_1252.h` & `libhmac-20240417/libuna/libuna_codepage_windows_1252.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_codepage_iso_8859_14.h` & `libhmac-20240417/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base16_stream.h` & `libhmac-20240417/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/libuna/libuna_base32_stream.c` & `libhmac-20240417/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libhmac-20240129/Makefile.in` & `libhmac-20240417/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -572,16 +572,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libhmac.pc \
+	libhmac.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libhmac.pc
 
 all: all-recursive
 
@@ -998,23 +1005,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1113,22 +1123,10 @@
 library:
 	(cd $(srcdir)/common && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcthreads && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libhmac.pc
-	-rm -f libhmac.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/pyhmac/pyhmac_md5_context.h` & `libhmac-20240417/pyhmac/pyhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac.h` & `libhmac-20240417/pyhmac/pyhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_libcerror.h` & `libhmac-20240417/pyhmac/pyhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_md5.c` & `libhmac-20240417/pyhmac/pyhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha1_context.h` & `libhmac-20240417/pyhmac/pyhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha256_context.h` & `libhmac-20240417/pyhmac/pyhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha224.h` & `libhmac-20240417/pyhmac/pyhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha1_context.c` & `libhmac-20240417/pyhmac/pyhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha256_context.c` & `libhmac-20240417/pyhmac/pyhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_unused.h` & `libhmac-20240417/pyhmac/pyhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha512_context.c` & `libhmac-20240417/pyhmac/pyhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha256.h` & `libhmac-20240417/pyhmac/pyhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha512.h` & `libhmac-20240417/pyhmac/pyhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha1.h` & `libhmac-20240417/pyhmac/pyhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_error.c` & `libhmac-20240417/pyhmac/pyhmac_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/Makefile.am` & `libhmac-20240417/pyhmac/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBHMAC_DLL_IMPORT@
 
 pyexec_LTLIBRARIES = pyhmac.la
 
 pyhmac_la_SOURCES = \
 	pyhmac.c pyhmac.h \
@@ -30,13 +30,11 @@
 	../libhmac/libhmac.la
 
 pyhmac_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyhmac_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha512.c` & `libhmac-20240417/pyhmac/pyhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_md5.h` & `libhmac-20240417/pyhmac/pyhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha1.c` & `libhmac-20240417/pyhmac/pyhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac.c` & `libhmac-20240417/pyhmac/pyhmac.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_libhmac.h` & `libhmac-20240417/pyhmac/pyhmac_libhmac.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha512_context.h` & `libhmac-20240417/pyhmac/pyhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha256.c` & `libhmac-20240417/pyhmac/pyhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha224_context.h` & `libhmac-20240417/pyhmac/pyhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha224_context.c` & `libhmac-20240417/pyhmac/pyhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_error.h` & `libhmac-20240417/pyhmac/pyhmac_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_python.h` & `libhmac-20240417/pyhmac/pyhmac_python.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/Makefile.in` & `libhmac-20240417/pyhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -508,16 +508,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBHMAC_DLL_IMPORT@
 
 @HAVE_PYTHON_TRUE@pyexec_LTLIBRARIES = pyhmac.la
 @HAVE_PYTHON_TRUE@pyhmac_la_SOURCES = \
 @HAVE_PYTHON_TRUE@	pyhmac.c pyhmac.h \
 @HAVE_PYTHON_TRUE@	pyhmac_error.c pyhmac_error.h \
@@ -538,15 +538,16 @@
 
 @HAVE_PYTHON_TRUE@pyhmac_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libhmac/libhmac.la
 
 @HAVE_PYTHON_TRUE@pyhmac_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyhmac_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -868,24 +869,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_error.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/pyhmac_la-pyhmac_sha512_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -981,13 +996,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libhmac-20240129/pyhmac/pyhmac_sha224.c` & `libhmac-20240417/pyhmac/pyhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/pyhmac/pyhmac_md5_context.c` & `libhmac-20240417/pyhmac/pyhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_definitions.h` & `libhmac-20240417/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libhmac-20240129/libcnotify/libcnotify_extern.h` & `libhmac-20240417/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_support.c` & `libhmac-20240417/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_stream.h` & `libhmac-20240417/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/Makefile.am` & `libhmac-20240417/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libhmac-20240129/libcnotify/libcnotify_unused.h` & `libhmac-20240417/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_verbose.h` & `libhmac-20240417/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_print.h` & `libhmac-20240417/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_stream.c` & `libhmac-20240417/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_support.h` & `libhmac-20240417/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_verbose.c` & `libhmac-20240417/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/Makefile.in` & `libhmac-20240417/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -457,30 +457,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -683,24 +684,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -787,17 +794,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/libcnotify/libcnotify_libcerror.h` & `libhmac-20240417/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcnotify/libcnotify_print.c` & `libhmac-20240417/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_system.c` & `libhmac-20240417/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_error.c` & `libhmac-20240417/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_extern.h` & `libhmac-20240417/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/Makefile.am` & `libhmac-20240417/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libhmac-20240129/libcerror/libcerror_types.h` & `libhmac-20240417/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_support.h` & `libhmac-20240417/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_error.h` & `libhmac-20240417/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_system.h` & `libhmac-20240417/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_definitions.h` & `libhmac-20240417/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libhmac-20240129/libcerror/libcerror_support.c` & `libhmac-20240417/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/libcerror_unused.h` & `libhmac-20240417/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/libcerror/Makefile.in` & `libhmac-20240417/libcerror/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -454,28 +454,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -677,24 +678,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -780,17 +786,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libhmac-20240129/aclocal.m4` & `libhmac-20240417/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libhmac-20240129/configure.ac` & `libhmac-20240417/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libhmac],
- [20240129],
+ [20240417],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libhmac.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

