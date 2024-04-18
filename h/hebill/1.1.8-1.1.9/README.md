# Comparing `tmp/hebill-1.1.8.tar.gz` & `tmp/hebill-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.1.8.tar", last modified: Fri Apr 12 01:05:39 2024, max compression
+gzip compressed data, was "hebill-1.1.9.tar", last modified: Thu Apr 18 02:40:51 2024, max compression
```

## Comparing `hebill-1.1.8.tar` & `hebill-1.1.9.tar`

### file list

```diff
@@ -1,302 +1,326 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.550431 hebill-1.1.8/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.8/LICENSE.rst
--rw-rw-rw-   0        0        0      487 2024-04-12 01:05:39.550431 hebill-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.327305 hebill-1.1.8/hebill/
--rw-rw-rw-   0        0        0      514 2024-04-12 00:54:52.000000 hebill-1.1.8/hebill/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.340825 hebill-1.1.8/hebill/dimensions/
--rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.1.8/hebill/dimensions/__init__.py
--rw-rw-rw-   0        0        0     1561 2024-04-11 08:59:34.000000 hebill-1.1.8/hebill/dimensions/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.345509 hebill-1.1.8/hebill/dir/
--rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.8/hebill/dir/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.8/hebill/dir/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.347522 hebill-1.1.8/hebill/excel/
--rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.1.8/hebill/excel/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.1.8/hebill/excel/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.351519 hebill-1.1.8/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.8/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.8/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.354923 hebill-1.1.8/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.357061 hebill-1.1.8/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.359088 hebill-1.1.8/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.8/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.360627 hebill-1.1.8/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.8/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.8/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.8/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.362636 hebill-1.1.8/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.8/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.8/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.364635 hebill-1.1.8/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.8/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.366635 hebill-1.1.8/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.8/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.8/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.367636 hebill-1.1.8/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.8/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.8/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.369674 hebill-1.1.8/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.8/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.8/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.370636 hebill-1.1.8/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.8/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.373153 hebill-1.1.8/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.8/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.375155 hebill-1.1.8/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.8/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.8/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.377576 hebill-1.1.8/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.8/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.378589 hebill-1.1.8/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.8/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.8/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.379586 hebill-1.1.8/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.381585 hebill-1.1.8/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.8/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.8/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.383587 hebill-1.1.8/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.8/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.8/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.384585 hebill-1.1.8/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.8/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.8/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.386876 hebill-1.1.8/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.8/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.8/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.388195 hebill-1.1.8/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.390205 hebill-1.1.8/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.8/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.8/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.8/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.392204 hebill-1.1.8/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.8/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.8/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.394204 hebill-1.1.8/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.8/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.8/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.396534 hebill-1.1.8/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.8/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.8/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.398113 hebill-1.1.8/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.8/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.400277 hebill-1.1.8/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.402437 hebill-1.1.8/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.405134 hebill-1.1.8/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.8/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.8/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.406356 hebill-1.1.8/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.408517 hebill-1.1.8/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.8/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.410086 hebill-1.1.8/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.8/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.411670 hebill-1.1.8/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.8/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.413680 hebill-1.1.8/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.414740 hebill-1.1.8/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.416750 hebill-1.1.8/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.417891 hebill-1.1.8/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.419900 hebill-1.1.8/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.420994 hebill-1.1.8/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.8/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.423006 hebill-1.1.8/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.8/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.424153 hebill-1.1.8/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.8/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.426163 hebill-1.1.8/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.8/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.427162 hebill-1.1.8/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.8/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.429162 hebill-1.1.8/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.8/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.430386 hebill-1.1.8/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.8/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.432385 hebill-1.1.8/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.8/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.433386 hebill-1.1.8/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.8/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.434893 hebill-1.1.8/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.8/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.436902 hebill-1.1.8/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.8/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.438902 hebill-1.1.8/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.8/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.440715 hebill-1.1.8/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.8/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.441730 hebill-1.1.8/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.8/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.8/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.442731 hebill-1.1.8/hebill/image/
--rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.1.8/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.447101 hebill-1.1.8/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.8/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.1.8/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.8/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.452121 hebill-1.1.8/hebill/mysql/
--rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.8/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.8/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.8/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.458121 hebill-1.1.8/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.460120 hebill-1.1.8/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.461925 hebill-1.1.8/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.8/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.8/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.462938 hebill-1.1.8/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.8/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.8/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.465345 hebill-1.1.8/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.8/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.8/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.469426 hebill-1.1.8/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.8/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.8/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.8/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.8/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.470436 hebill-1.1.8/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.472862 hebill-1.1.8/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.8/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.479175 hebill-1.1.8/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.8/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.8/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.8/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.8/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.8/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.8/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.483307 hebill-1.1.8/hebill/numeric/
--rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.1.8/hebill/numeric/__init__.py
--rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.1.8/hebill/numeric/constants.py
--rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.1.8/hebill/numeric/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.487215 hebill-1.1.8/hebill/pdf/
--rw-rw-rw-   0        0        0      309 2024-04-09 02:09:58.000000 hebill-1.1.8/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.489223 hebill-1.1.8/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.8/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/component/core.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.8/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8079 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.494224 hebill-1.1.8/hebill/pdf/features/
--rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.1.8/hebill/pdf/features/__init__.py
--rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/features/configs.py
--rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/features/document_configs.py
--rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/features/page_configs.py
--rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/features/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.499282 hebill-1.1.8/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.8/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.8/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.8/hebill/pdf/library/configs_selector_font.py
--rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.8/hebill/pdf/library/get_display_width.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.514698 hebill-1.1.8/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.8/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.8/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.8/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.8/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.1.8/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.8/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.8/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.8/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.8/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.8/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.8/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.8/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.516826 hebill-1.1.8/hebill/pypi/
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.8/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     7849 2024-04-09 01:50:41.000000 hebill-1.1.8/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.518961 hebill-1.1.8/hebill/string/
--rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.1.8/hebill/string/__init__.py
--rw-rw-rw-   0        0        0     1517 2024-04-10 08:10:15.000000 hebill-1.1.8/hebill/string/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.521115 hebill-1.1.8/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.8/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.8/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.523811 hebill-1.1.8/hebill/tyre/
--rw-rw-rw-   0        0        0       24 2024-04-11 03:10:12.000000 hebill-1.1.8/hebill/tyre/__init__.py
--rw-rw-rw-   0        0        0      920 2024-04-11 08:39:33.000000 hebill-1.1.8/hebill/tyre/constansts.py
--rw-rw-rw-   0        0        0     5532 2024-04-11 08:43:02.000000 hebill-1.1.8/hebill/tyre/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.525821 hebill-1.1.8/hebill/tyre/features/
--rw-rw-rw-   0        0        0        0 2024-04-11 01:24:59.000000 hebill-1.1.8/hebill/tyre/features/__init__.py
--rw-rw-rw-   0        0        0     6114 2024-04-11 08:59:34.000000 hebill-1.1.8/hebill/tyre/features/dimensions.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.528333 hebill-1.1.8/hebill/tyre_mould/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:43:22.000000 hebill-1.1.8/hebill/tyre_mould/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.530346 hebill-1.1.8/hebill/tyre_mould/components/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:45:12.000000 hebill-1.1.8/hebill/tyre_mould/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.533869 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_lower/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:46:58.000000 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_lower/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-11 08:49:20.000000 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_lower/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.535869 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_middle/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:47:04.000000 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_middle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.537873 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_upper/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:46:26.000000 hebill-1.1.8/hebill/tyre_mould/components/bead_ring_upper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.538872 hebill-1.1.8/hebill/tyre_mould/components/clamp_ring_lower/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:47:23.000000 hebill-1.1.8/hebill/tyre_mould/components/clamp_ring_lower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.539868 hebill-1.1.8/hebill/tyre_mould/components/clamp_ring_upper/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:47:39.000000 hebill-1.1.8/hebill/tyre_mould/components/clamp_ring_upper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.541353 hebill-1.1.8/hebill/tyre_mould/components/mould_body_2_pieces_lower/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:46:02.000000 hebill-1.1.8/hebill/tyre_mould/components/mould_body_2_pieces_lower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.541353 hebill-1.1.8/hebill/tyre_mould/components/mould_body_2_pieces_upper/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:45:34.000000 hebill-1.1.8/hebill/tyre_mould/components/mould_body_2_pieces_upper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.542365 hebill-1.1.8/hebill/tyre_mould/components/sidewall_plate_lower/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:48:35.000000 hebill-1.1.8/hebill/tyre_mould/components/sidewall_plate_lower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.543390 hebill-1.1.8/hebill/tyre_mould/components/sidewall_plate_upper/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:48:21.000000 hebill-1.1.8/hebill/tyre_mould/components/sidewall_plate_upper/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:51:54.000000 hebill-1.1.8/hebill/tyre_mould/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.545397 hebill-1.1.8/hebill/tyre_mould/features/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:49:29.000000 hebill-1.1.8/hebill/tyre_mould/features/__init__.py
--rw-rw-rw-   0        0        0      287 2024-04-11 09:04:13.000000 hebill-1.1.8/hebill/tyre_mould/features/mould_2ps_half_dimensions.py
--rw-rw-rw-   0        0        0      809 2024-04-11 09:04:13.000000 hebill-1.1.8/hebill/tyre_mould/features/ring_dimensions.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.548399 hebill-1.1.8/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.8/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.8/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:05:39.548399 hebill-1.1.8/hebill.egg-info/
--rw-rw-rw-   0        0        0      487 2024-04-12 01:05:39.000000 hebill-1.1.8/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7256 2024-04-12 01:05:39.000000 hebill-1.1.8/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 01:05:39.000000 hebill-1.1.8/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-12 01:05:39.000000 hebill-1.1.8/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 01:05:39.000000 hebill-1.1.8/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2024-04-12 01:05:39.551439 hebill-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      524 2024-04-12 01:05:38.000000 hebill-1.1.8/setup_by_hebill.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.446513 hebill-1.1.9/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.9/LICENSE.rst
+-rw-rw-rw-   0        0        0      487 2024-04-18 02:40:51.446513 hebill-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.162270 hebill-1.1.9/hebill/
+-rw-rw-rw-   0        0        0      555 2024-04-18 02:40:49.000000 hebill-1.1.9/hebill/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.187798 hebill-1.1.9/hebill/dimensions/
+-rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.1.9/hebill/dimensions/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.1.9/hebill/dimensions/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.191819 hebill-1.1.9/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.9/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.9/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.194897 hebill-1.1.9/hebill/excel/
+-rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.1.9/hebill/excel/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.1.9/hebill/excel/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.199748 hebill-1.1.9/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.9/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.9/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.201742 hebill-1.1.9/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.203761 hebill-1.1.9/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.205758 hebill-1.1.9/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.9/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.207749 hebill-1.1.9/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.9/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.9/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.9/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.208720 hebill-1.1.9/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.9/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.9/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.211589 hebill-1.1.9/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.9/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.213582 hebill-1.1.9/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.9/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.9/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.214991 hebill-1.1.9/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.9/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.9/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.216989 hebill-1.1.9/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.9/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.9/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.218983 hebill-1.1.9/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.9/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.220976 hebill-1.1.9/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.9/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.222045 hebill-1.1.9/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.9/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.9/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.224038 hebill-1.1.9/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.9/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.225035 hebill-1.1.9/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.9/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.9/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.226539 hebill-1.1.9/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.227540 hebill-1.1.9/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.9/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.9/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.229597 hebill-1.1.9/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.9/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.9/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.230598 hebill-1.1.9/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.9/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.9/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.231928 hebill-1.1.9/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.9/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.9/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.233925 hebill-1.1.9/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.235361 hebill-1.1.9/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.9/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.9/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.9/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.237358 hebill-1.1.9/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.9/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.9/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.238355 hebill-1.1.9/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.9/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.9/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.244852 hebill-1.1.9/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.9/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.9/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.246369 hebill-1.1.9/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.9/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.253334 hebill-1.1.9/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.255331 hebill-1.1.9/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.256328 hebill-1.1.9/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.9/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.9/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.259314 hebill-1.1.9/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.262854 hebill-1.1.9/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.9/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.264925 hebill-1.1.9/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.9/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.266889 hebill-1.1.9/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.9/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.269880 hebill-1.1.9/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.271877 hebill-1.1.9/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.273871 hebill-1.1.9/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.276857 hebill-1.1.9/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.277854 hebill-1.1.9/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.279847 hebill-1.1.9/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.9/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.282018 hebill-1.1.9/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.9/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.284007 hebill-1.1.9/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.9/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.285521 hebill-1.1.9/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.9/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.287027 hebill-1.1.9/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.9/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.288024 hebill-1.1.9/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.9/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.290527 hebill-1.1.9/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.9/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.292882 hebill-1.1.9/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.9/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.293878 hebill-1.1.9/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.9/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.295870 hebill-1.1.9/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.9/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.296868 hebill-1.1.9/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.9/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.299172 hebill-1.1.9/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.9/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.301169 hebill-1.1.9/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.9/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.302675 hebill-1.1.9/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.9/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.9/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.303671 hebill-1.1.9/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.1.9/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.307495 hebill-1.1.9/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.9/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.1.9/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.9/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.310096 hebill-1.1.9/hebill/math/
+-rw-rw-rw-   0        0        0       52 2024-04-16 07:28:38.000000 hebill-1.1.9/hebill/math/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-16 07:28:38.000000 hebill-1.1.9/hebill/math/ring_volume_weight.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.311497 hebill-1.1.9/hebill/mould/
+-rw-rw-rw-   0        0        0      116 2024-04-15 00:57:06.000000 hebill-1.1.9/hebill/mould/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.316302 hebill-1.1.9/hebill/mould/tyre_mould/
+-rw-rw-rw-   0        0        0        0 2024-04-13 02:19:53.000000 hebill-1.1.9/hebill/mould/tyre_mould/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.317298 hebill-1.1.9/hebill/mould/tyre_mould/components/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:45:12.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.318294 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_lower/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:46:58.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_lower/__init__.py
+-rw-rw-rw-   0        0        0     1255 2024-04-17 01:31:18.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_lower/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.320288 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_middle/
+-rw-rw-rw-   0        0        0        0 2024-04-12 01:22:09.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_middle/__init__.py
+-rw-rw-rw-   0        0        0     1281 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_middle/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.322791 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_upper/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:46:26.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_upper/__init__.py
+-rw-rw-rw-   0        0        0     1262 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/bead_ring_upper/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.324785 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_lower/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:47:23.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_lower/__init__.py
+-rw-rw-rw-   0        0        0     1250 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_lower/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.326777 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_upper/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:47:39.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_upper/__init__.py
+-rw-rw-rw-   0        0        0     1248 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/clamp_ring_upper/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.328771 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_center_spacer/
+-rw-rw-rw-   0        0        0        0 2024-04-12 01:17:57.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_center_spacer/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_center_spacer/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.332275 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_lower/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:46:02.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_lower/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-17 01:18:54.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_lower/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.334272 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_upper/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:45:34.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_upper/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-17 01:18:54.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/mould_2ps_half_upper/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.339341 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_lower/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:48:35.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_lower/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_lower/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.342467 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_upper/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:48:21.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_upper/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-17 01:29:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/components/sidewall_plate_upper/core.py
+-rw-rw-rw-   0        0        0      568 2024-04-15 15:50:46.000000 hebill-1.1.9/hebill/mould/tyre_mould/constants.py
+-rw-rw-rw-   0        0        0     5395 2024-04-17 01:36:39.000000 hebill-1.1.9/hebill/mould/tyre_mould/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.355478 hebill-1.1.9/hebill/mould/tyre_mould/features/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:49:29.000000 hebill-1.1.9/hebill/mould/tyre_mould/features/__init__.py
+-rw-rw-rw-   0        0        0     1733 2024-04-16 01:06:00.000000 hebill-1.1.9/hebill/mould/tyre_mould/features/mould_2ps_dimensions.py
+-rw-rw-rw-   0        0        0     4412 2024-04-17 02:16:16.000000 hebill-1.1.9/hebill/mould/tyre_mould/features/mould_2ps_half.py
+-rw-rw-rw-   0        0        0     1401 2024-04-17 01:30:22.000000 hebill-1.1.9/hebill/mould/tyre_mould/features/ring_component.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.359464 hebill-1.1.9/hebill/mould/tyre_mould/methods/
+-rw-rw-rw-   0        0        0        0 2024-04-13 08:55:23.000000 hebill-1.1.9/hebill/mould/tyre_mould/methods/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-04-15 15:25:32.000000 hebill-1.1.9/hebill/mould/tyre_mould/methods/mould_2pcs_horizontal_thickness.py
+-rw-rw-rw-   0        0        0      351 2024-04-15 15:45:47.000000 hebill-1.1.9/hebill/mould/tyre_mould/methods/mould_2pcs_vertical_thickness.py
+-rw-rw-rw-   0        0        0     7537 2024-04-17 01:36:39.000000 hebill-1.1.9/hebill/mould/tyre_mould/mould_two_pieces.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.362962 hebill-1.1.9/hebill/mysql/
+-rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.9/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.9/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.9/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.368479 hebill-1.1.9/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.370473 hebill-1.1.9/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.371469 hebill-1.1.9/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.9/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.9/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.373966 hebill-1.1.9/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.9/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.9/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.376121 hebill-1.1.9/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.9/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.9/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.380883 hebill-1.1.9/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.9/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.9/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.9/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.9/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.382438 hebill-1.1.9/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.385195 hebill-1.1.9/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.9/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.391883 hebill-1.1.9/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.9/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.9/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.9/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.9/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.9/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.9/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.396112 hebill-1.1.9/hebill/numeric/
+-rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.1.9/hebill/numeric/__init__.py
+-rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.1.9/hebill/numeric/constants.py
+-rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.1.9/hebill/numeric/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.401256 hebill-1.1.9/hebill/pdf/
+-rw-rw-rw-   0        0        0      309 2024-04-09 02:09:58.000000 hebill-1.1.9/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.402253 hebill-1.1.9/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.9/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/component/core.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.9/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8079 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.408683 hebill-1.1.9/hebill/pdf/features/
+-rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.1.9/hebill/pdf/features/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/features/configs.py
+-rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/features/document_configs.py
+-rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/features/page_configs.py
+-rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/features/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.415177 hebill-1.1.9/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.9/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.9/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.9/hebill/pdf/library/configs_selector_font.py
+-rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.9/hebill/pdf/library/get_display_width.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.430152 hebill-1.1.9/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.9/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.9/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.9/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.9/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.1.9/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.9/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.9/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.9/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.9/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.9/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.9/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.9/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.432145 hebill-1.1.9/hebill/pypi/
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.9/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2024-04-09 01:50:41.000000 hebill-1.1.9/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.434697 hebill-1.1.9/hebill/string/
+-rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.1.9/hebill/string/__init__.py
+-rw-rw-rw-   0        0        0     1571 2024-04-16 02:09:46.000000 hebill-1.1.9/hebill/string/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.436054 hebill-1.1.9/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.9/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      400 2024-04-18 02:40:49.000000 hebill-1.1.9/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.439617 hebill-1.1.9/hebill/tyre/
+-rw-rw-rw-   0        0        0       24 2024-04-11 03:10:12.000000 hebill-1.1.9/hebill/tyre/__init__.py
+-rw-rw-rw-   0        0        0      915 2024-04-15 03:20:04.000000 hebill-1.1.9/hebill/tyre/constansts.py
+-rw-rw-rw-   0        0        0     5451 2024-04-16 02:32:49.000000 hebill-1.1.9/hebill/tyre/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.442313 hebill-1.1.9/hebill/tyre/features/
+-rw-rw-rw-   0        0        0        0 2024-04-11 01:24:59.000000 hebill-1.1.9/hebill/tyre/features/__init__.py
+-rw-rw-rw-   0        0        0     6855 2024-04-16 02:27:12.000000 hebill-1.1.9/hebill/tyre/features/tyre.py
+-rw-rw-rw-   0        0        0      697 2024-04-15 16:13:40.000000 hebill-1.1.9/hebill/tyre/features/tyre_dimensions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.444306 hebill-1.1.9/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.9/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.9/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:40:51.445303 hebill-1.1.9/hebill.egg-info/
+-rw-rw-rw-   0        0        0      487 2024-04-18 02:40:50.000000 hebill-1.1.9/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8394 2024-04-18 02:40:51.000000 hebill-1.1.9/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:40:50.000000 hebill-1.1.9/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-18 02:40:50.000000 hebill-1.1.9/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 02:40:50.000000 hebill-1.1.9/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2024-04-18 02:40:51.447510 hebill-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      524 2024-04-18 02:40:50.000000 hebill-1.1.9/setup_by_hebill.py
```

### Comparing `hebill-1.1.8/hebill/__init__.py` & `hebill-1.1.9/hebill/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from . import dimensions
 from . import dir
 from . import excel
 from . import file
 from . import html
 from . import image
+from . import math
+from . import mould
 from . import mysql
 from . import numeric
 from . import pdf
 from . import pypi
 from . import string
 from . import sys
 from . import tyre
 from . import url
 
-app_version = '1.1.8'
+app_version = '1.1.9'
 app_name = 'hebill'
 app_description = 'Python Hebill'
 app_url = 'http://www.hebill.net/'
 app_author = 'He Bill'
 app_author_email = 'hebill@hebill.net'
 app_author_url = 'http://www.hebill.net/'
```

### Comparing `hebill-1.1.8/hebill/dimensions/core.py` & `hebill-1.1.9/hebill/dimensions/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,7 +34,13 @@
                     self._error = f'Value of {value} is string, but nor not digitalizable.'
             elif value is None:
                 super().__setitem__(key, None)
             else:
                 self._error = f'Value type of {value} is not supported.'
         else:
             self._error = f'Key name {key} is not supported.'
+
+    def all_available(self):
+        for n, v, in self.items():
+            if v is None:
+                return False
+        return True
```

### Comparing `hebill-1.1.8/hebill/dir/core.py` & `hebill-1.1.9/hebill/dir/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/file/core.py` & `hebill-1.1.9/hebill/file/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/html/head/core.py` & `hebill-1.1.9/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/table/core.py` & `hebill-1.1.9/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/table/tbody/core.py` & `hebill-1.1.9/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.1.9/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/table/thead/core.py` & `hebill-1.1.9/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/components/table/thead/tr/core.py` & `hebill-1.1.9/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/core.py` & `hebill-1.1.9/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/comment/core.py` & `hebill-1.1.9/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/group/core.py` & `hebill-1.1.9/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/group/create/core.py` & `hebill-1.1.9/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.1.9/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.1.9/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/node/core.py` & `hebill-1.1.9/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.1.9/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.1.9/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.1.9/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/nodes/tag/core.py` & `hebill-1.1.9/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/html/tags/__init__.py` & `hebill-1.1.9/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/image/__init__.py` & `hebill-1.1.9/hebill/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/image/png/constants.py` & `hebill-1.1.9/hebill/image/png/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/image/png/core.py` & `hebill-1.1.9/hebill/image/png/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/core.py` & `hebill-1.1.9/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/features/table_describe_data.py` & `hebill-1.1.9/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/features/table_index_data.py` & `hebill-1.1.9/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/features/table_status_data.py` & `hebill-1.1.9/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/plugins/columns/core.py` & `hebill-1.1.9/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/plugins/limits/core.py` & `hebill-1.1.9/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/plugins/orders/core.py` & `hebill-1.1.9/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.1.9/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.1.9/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/core.py` & `hebill-1.1.9/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/data/core.py` & `hebill-1.1.9/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/data/drop.py` & `hebill-1.1.9/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/data/insert.py` & `hebill-1.1.9/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/data/search.py` & `hebill-1.1.9/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/mysql/table/data/update.py` & `hebill-1.1.9/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/numeric/constants.py` & `hebill-1.1.9/hebill/numeric/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/numeric/core.py` & `hebill-1.1.9/hebill/numeric/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/component/core.py` & `hebill-1.1.9/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/constants.py` & `hebill-1.1.9/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/core.py` & `hebill-1.1.9/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/features/document_configs.py` & `hebill-1.1.9/hebill/pdf/features/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/features/page_configs.py` & `hebill-1.1.9/hebill/pdf/features/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/features/styles.py` & `hebill-1.1.9/hebill/pdf/features/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/library/configs_selector_color.py` & `hebill-1.1.9/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/library/configs_selector_font.py` & `hebill-1.1.9/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/library/get_display_width.py` & `hebill-1.1.9/hebill/pdf/library/get_display_width.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/_draw_.py` & `hebill-1.1.9/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/core.py` & `hebill-1.1.9/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/draw_grids.py` & `hebill-1.1.9/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/draw_path.py` & `hebill-1.1.9/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/draw_rect.py` & `hebill-1.1.9/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pdf/page/draw_string.py` & `hebill-1.1.9/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/pypi/core.py` & `hebill-1.1.9/hebill/pypi/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.8/hebill/string/core.py` & `hebill-1.1.9/hebill/string/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
                 return None if return_number else False
         if not return_number:
             return True
         integer_part = integer_part.replace(',', '')
         if is_float:
             number = float(f'{integer_part}.{decimal_part if len(decimal_part) > 0 else 0}')
             return number if not negative else -number
+        if integer_part == '':
+            return 0
         return int(integer_part)
 
     def digitalizable(self) -> bool:
         return self._digitize()
 
     def digitize(self):
         return self._digitize(True)
```

### Comparing `hebill-1.1.8/hebill/tyre/constansts.py` & `hebill-1.1.9/hebill/tyre/constansts.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # 最大印制直径
 # 目前参考 65/65-65
 SIZE_MAX_DIAMETER_INCH = 65
 RATIO_RW_TO_SW = .8
 RATIO_NSD_TO_SW = .07
 SIZE_DEFAULT_ASPECT_RATIO = .95
 SIZE_DEFAULT_ASPECT_RATIOS = {
-    "5.00-8": 1,
-    "5.50-16": 1.1,
-    "10-16.5": .7,
-    "11L-16": .7,
-    "11.2-24": .95,
-    "11.2-28": .95,
-    "12-16.5": .7,
-    "12.4-28": .95,
-    "13.6-24": .9,
-    "13.6-28": .95,
-    "14.9-24": .9,
-    "14.9-28": .95,
-    "16.9-24": .9,
-    "16.9-28": .95,
-    '18.4/15-30': .89,
-    "19.5-24": .7,
-    "37.25-35": .8,
-    "40.00-57": 1,
-    "165R16": .75,
-    "175R16": .75,
+    "5.00-8": 100,
+    "5.50-16": 110,
+    "10-16.5": 70,
+    "11L-16": 70,
+    "11.2-24": 95,
+    "11.2-28": 95,
+    "12-16.5": 70,
+    "12.4-28": 95,
+    "13.6-24": 90,
+    "13.6-28": 95,
+    "14.9-24": 90,
+    "14.9-28": 95,
+    "16.9-24": 90,
+    "16.9-28": 95,
+    '18.4/15-30': 89,
+    "19.5-24": 70,
+    "37.25-35": 80,
+    "40.00-57": 100,
+    "165R16": 75,
+    "175R16": 75,
 }
```

### Comparing `hebill-1.1.8/hebill/tyre/core.py` & `hebill-1.1.9/hebill/tyre/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from .features.dimensions import Dimensions
+from .features.tyre import Tyre as ObjectTPL
 from .constansts import SIZE_DEFAULT_ASPECT_RATIOS, RATIO_NSD_TO_SW, RATIO_RW_TO_SW, SIZE_DEFAULT_ASPECT_RATIO
 
 
-class Tyre(Dimensions):
+class Tyre(ObjectTPL):
     def __init__(self, size, dimensions: dict = None):
         self._primary = None
         self._secondary = None
         super().__init__(size, dimensions)
-
         if self.rim_size is None:
             if self.primary.rim_size is not None:
                 self.rim_size = self.primary.rim_size
             elif self.secondary.rim_size is not None:
                 self.rim_size = self.secondary.rim_size
 
         if self.rim_diameter is None:
             if self.rim_size is not None:
                 self.rim_diameter = self.rim_size * 25.4
             elif self.primary.rim_diameter is not None:
                 self.rim_diameter = self.primary.rim_diameter
             elif self.secondary.rim_diameter is not None:
                 self.rim_diameter = self.secondary.rim_diameter
-
         if self.aspect_ratio is None:
             if self.diameter is not None and self.section_width is not None and self.rim_diameter is not None:
-                self.aspect_ratio = round((self.diameter - self.rim_diameter) / 2 / self.section_width, 2) * 100
+                self.aspect_ratio = round((self.diameter - self.rim_diameter) / 2 / self.section_width, 4) * 100
             elif self.primary.aspect_ratio is not None:
                 self.aspect_ratio = self.primary.aspect_ratio
             elif self.secondary.aspect_ratio is not None:
                 self.aspect_ratio = self.secondary.aspect_ratio
             else:
                 self.aspect_ratio = SIZE_DEFAULT_ASPECT_RATIO
 
@@ -45,22 +43,18 @@
                 self.section_width = (self.diameter - self.rim_diameter) / 2 / self.aspect_ratio * 100
             elif self.primary.section_width is not None:
                 self.section_width = self.primary.section_width
             elif self.secondary.section_width is not None:
                 self.section_width = self.secondary.section_width
 
         if self.section_width is not None:
-            self.non_skid_depth = round(self.section_width * RATIO_NSD_TO_SW, 2)
-            self.rim_width = round(self.section_width * RATIO_RW_TO_SW)
-
-    def all_dimensions_available(self):
-        for n, v, in self.items():
-            if v is None:
-                return False
-        return True
+            if self.non_skid_depth is None:
+                self.non_skid_depth = round(self.section_width * RATIO_NSD_TO_SW, 2)
+            if self.rim_width is None:
+                self.rim_width = round(self.section_width * RATIO_RW_TO_SW)
 
     @property
     def size_formatted(self) -> str:
         if self.secondary.size:
             return '|'.join([self.primary.size, self.secondary.size])
         return self.primary.size
 
@@ -72,47 +66,43 @@
         if secondary['rim_size_perfect'] and not secondary['rim_size_perfect']:
             primary['rim_size'] = secondary['rim_size']
         if primary['aspect_ratio_perfect'] and not secondary['aspect_ratio_perfect']:
             secondary['aspect_ratio'] = primary['aspect_ratio']
         if secondary['aspect_ratio_perfect'] and not primary['aspect_ratio_perfect']:
             primary['aspect_ratio'] = secondary['aspect_ratio']
 
-        def workout(d: Dimensions):
+        def workout(d: ObjectTPL):
             if d.rim_diameter is None:
                 if d.rim_size is not None:
                     d.rim_diameter = d.rim_size * 25.4
-
             if d.aspect_ratio is None:
                 if d.diameter is not None and d.section_width is not None and d.rim_diameter is not None:
                     d.aspect_ratio = round((d.diameter - d.rim_diameter) / 2 / d.section_width, 2) * 100
                 elif d.size in SIZE_DEFAULT_ASPECT_RATIOS:
                     d.aspect_ratio = SIZE_DEFAULT_ASPECT_RATIOS[d.size]
                 else:
                     d.aspect_ratio = 96
-
             if d.diameter is None:
                 if d.section_width is not None and d.rim_diameter is not None:
                     d.diameter = d.section_width * d.aspect_ratio * 2 / 100 + d.rim_diameter
-
             if d.section_width is None:
                 if d.diameter is not None and d.rim_diameter is not None:
                     d.section_width = (d.diameter - d.rim_diameter) / 2 / d.aspect_ratio * 100
-
             if d.section_width is not None:
                 d.non_skid_depth = round(d.section_width * RATIO_NSD_TO_SW, 2)
                 d.rim_width = round(d.section_width * RATIO_RW_TO_SW)
-        self._primary = Dimensions(primary['size'], primary)
-        self._secondary = Dimensions(secondary['size'], secondary)
+        self._primary = ObjectTPL(primary['size'], primary)
+        self._secondary = ObjectTPL(secondary['size'], secondary)
         workout(self.primary)
         workout(self.secondary)
 
     @property
-    def primary(self) -> Dimensions:
+    def primary(self) -> ObjectTPL:
         if self._primary is None:
             self._primary_secondary()
         return self._primary
 
     @property
-    def secondary(self) -> Dimensions:
+    def secondary(self) -> ObjectTPL:
         if self._secondary is None:
             self._primary_secondary()
         return self._secondary
```

### Comparing `hebill-1.1.8/hebill/tyre/features/dimensions.py` & `hebill-1.1.9/hebill/tyre/features/tyre.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from ...dimensions.core import Dimensions as DimensionsTPL
 from ...string.core import String
 from ..constansts import (SIZE_SYMBOLS, SIZE_MAX_RIM_SIZE_INCH, SIZE_MAX_SECTION_WIDTH_INCH,
                           SIZE_MIN_ASPECT_RATIO, SIZE_MAX_ASPECT_RATIO, SIZE_MAX_DIAMETER_INCH)
+from .tyre_dimensions import TyreDimensions
 
 
-class Dimensions(DimensionsTPL):
+class Tyre(DimensionsTPL):
     names = ['diameter', 'section_width', 'non_skid_depth', 'aspect_ratio', 'rim_size', 'rim_diameter', 'rim_width']
 
     def __init__(self, size, dimensions: dict = None):
         super().__init__(dimensions)
         self._size = size
         self._error = ''
 
@@ -147,7 +148,27 @@
                     data['diameter_perfect'] = od > SIZE_MAX_DIAMETER_INCH
                     data['diameter'] = od if od > SIZE_MAX_DIAMETER_INCH else round(od * 25.4, 3)
                 if isinstance(data['middle'], str):
                     sw = String(data['middle']).digitize()
                     data['section_width_perfect'] = sw > SIZE_MAX_SECTION_WIDTH_INCH
                     data['section_width'] = sw if sw > SIZE_MAX_SECTION_WIDTH_INCH else round(sw * 25.4, 3)
         return data
+
+    @property
+    def dimensions(self):
+        return TyreDimensions({
+            'diameter': self.diameter,
+            'section_width': self.section_width,
+            'non_skid_depth': self.non_skid_depth,
+            'aspect_ratio': self.aspect_ratio,
+            'rim_size': self.rim_size,
+            'rim_diameter': self.rim_diameter,
+            'rim_width': self.rim_width,
+        })
+
+    @property
+    def dimensions_formatted(self):
+        dimensions = self.dimensions
+        for k, v in dimensions.items():
+            if isinstance(v, float) and len(str(v).split('.')[1]) > 2:
+                dimensions[k] = round(v, 2)
+        return TyreDimensions(dimensions)
```

### Comparing `hebill-1.1.8/setup_by_hebill.py` & `hebill-1.1.9/setup_by_hebill.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(
     name='hebill',
-    version='1.1.8',
+    version='1.1.9',
     description='Python Hebill',
     long_description=open(r'E:\PythonProjects\hebill\README.MD').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
```

