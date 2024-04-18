# Comparing `tmp/dataforgetoolkit-1.0.4-py3-none-any.whl.zip` & `tmp/dataforgetoolkit-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4093 bytes, number of entries: 7
+Zip file size: 4657 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      875 b- defN 24-Apr-17 09:58 dataforgetoolkit/__init__.py
 -rw-r--r--  2.0 unx      212 b- defN 24-Apr-17 09:19 dataforgetoolkit/common_utils.py
 -rw-r--r--  2.0 unx     3929 b- defN 24-Apr-17 15:00 dataforgetoolkit/datamapper.py
--rw-r--r--  2.0 unx     2003 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      593 b- defN 24-Apr-17 15:05 dataforgetoolkit-1.0.4.dist-info/RECORD
-7 files, 7721 bytes uncompressed, 3031 bytes compressed:  60.7%
+-rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 16:24 dataforgetoolkit-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:24 dataforgetoolkit-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 16:24 dataforgetoolkit-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-17 16:24 dataforgetoolkit-1.0.5.dist-info/RECORD
+7 files, 9135 bytes uncompressed, 3595 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: dataforgetoolkit/common_utils.py
 Comment: 
 
 Filename: dataforgetoolkit/datamapper.py
 Comment: 
 
-Filename: dataforgetoolkit-1.0.4.dist-info/METADATA
+Filename: dataforgetoolkit-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: dataforgetoolkit-1.0.4.dist-info/WHEEL
+Filename: dataforgetoolkit-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: dataforgetoolkit-1.0.4.dist-info/top_level.txt
+Filename: dataforgetoolkit-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dataforgetoolkit-1.0.4.dist-info/RECORD
+Filename: dataforgetoolkit-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dataforgetoolkit-1.0.4.dist-info/METADATA` & `dataforgetoolkit-1.0.5.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforgetoolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: It is a library that facilitates converting CSV files to various formats (such as DataFrames or other CSV/Excel files) based on a JSON mapping
 Home-page: https://github.com/amitsingh7668/dataforgetoolkit
 Author: Amit Singh
 Author-email: 2singh.amit3@gmail.com
 License: Amit Singh
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -16,32 +16,52 @@
 Description-Content-Type: text/markdown
 
 
 # Project Title
 
 DataForgeToolkit is a Python library for mapping CSV or Excel files based on JSON transformation mappings.
 
+# Description
 
-## Installation
+DataForgeToolkit: Flexible Data Mapping for CSV/XLSX Files
+
+The DataForgeToolkit is a Python library designed to streamline the process of converting CSV or Excel files into customized DataFrames based on user-defined JSON mapping configurations. Whether you're working with financial reports, customer datasets, or any other structured data, this toolkit empowers you to effortlessly transform raw data into actionable insights.
+
+Features:
+Versatile File Support: Seamlessly process both CSV and Excel files, providing flexibility in handling various data formats commonly encountered in data analysis tasks.
+
+Customizable Mapping: Define transformation mappings using a JSON file, allowing for precise specification of column names, data cleaning, and value substitutions tailored to your specific data requirements.
+
+Efficient Data Processing: Automate data preprocessing tasks such as handling missing values, standardizing column names, and applying complex value mappings with ease.
+
+
+## Installation Usage/Examples
 
-Install my-project with npm
 
 ```bash
   pip install dataforgetoolkit
 ```
 
-## Usage/Examples
+Define Transformation Mapping:
 
-```python
-    from dataforgetoolkit import datamapper
+Create a JSON file specifying the transformation mappings for your data. Define column mappings, specify new column names, and define value substitutions as needed.
+
+Use the Toolkit:
 
-    mapped_data = datamapper.map(report_file_path, transformation_file_path)
+Import the DataForgeToolkit in your Python script and utilize the map function to convert your report files:
 
+```bash
+    from dataforgetoolkit import datamapper
+    datamapper.map('report file path csv / xlsx format','mapping json file path')
 ```
 
+Access Mapped Data:
+
+Access the transformed data as a DataFrame for further analysis or export to other formats.
+
 
 ## JSON Transformation Mapping
 
  Transformation mappings are specified using a JSON file. Example:
 
     {
         "transformation_mapping": [
```

