# Comparing `tmp/Seq2SeqSharp-2.7.6.tar.gz` & `tmp/Seq2SeqSharp-2.8.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Seq2SeqSharp-2.7.6.tar", last modified: Fri May  5 06:18:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

