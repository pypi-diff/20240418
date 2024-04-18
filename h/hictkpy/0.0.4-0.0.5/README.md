# Comparing `tmp/hictkpy-0.0.4.tar.gz` & `tmp/hictkpy-0.0.5-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hictkpy-0.0.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

