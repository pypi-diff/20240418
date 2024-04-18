# Comparing `tmp/odoo14-addon-energy_project-14.0.3.1.0.tar.gz` & `tmp/odoo14_addon_energy_project-14.0.3.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_project-14.0.3.1.0.tar", last modified: Thu Mar  7 15:15:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
